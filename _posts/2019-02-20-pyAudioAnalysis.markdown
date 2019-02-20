---
layout:     post
title:      "音频分析工具包：pyAudioAnalysis中文文档"
subtitle:   " \"一个非常好用且强大的音频分析开源工具\""
date:       2019-02-20 16:30:00
author:     "mujiang"
header-img: "img/tools.jpg"
catalog: false
tags:
     - 技术

---

> “ `pyAudioAnalysis`是一个非常好用且强大的音频分析开源工具，能实现音频的特征提取、分类和回归模型的训练和执行，以及其他一些实用的功能。有些英文只能意会，翻译过来比较蹩脚，还请谅解。”

> “此工具也有一篇对应的论文做了介绍，可以免费下载。 [点击查看](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0144610)”
---


[TOC]

---

## 1.欢迎

欢迎使用pyAudioAnalysis.
pyAudioAnalysis是一个开源的Python库，提供了一系列音频分析相关的功能，主要包括：特征抽取、分类、分割和可视化。

## 2.简介

### 项目下载


```git
git clone https://github.com/tyiannak/pyAudioAnalysis.git
```

### 依赖

pyAudioAnalysis.git主要依赖以下几个库，使用pip或者IDE插件均可以安装。不再赘述。

* NUMPY
* MATPLOTLIB
* SCIPY
* SKLEARN
* hmmlearn
* Simplejson
* eyeD3
* pydub

### 核心库及其描述

* `audioAnalysis.py`: 主要实现了对命令行语句的执行
* `audioFeatureExtraction.py`: 实现了音频特征抽取的全部功能。包括：一共21个短期时长的特征及计算。此外，为了抽取音频特征的统计特性，也实现了一个中期时长窗口的特征计算。
* `audioTrainTest.py`: 实现了音频分类的过程。可以使用SVM和KNN分类器进行模型训练。此外还提供了方法的封装和常用的训练、评估、特征标准化等工具
* `audioSegmentation.py`: 实现了音频切割的功能，比如固定大小的分割、演讲者数字化等
* `audioBasicIO.py`: 主要提供了一些对音频文件的基础IO操作，如文件读取、格式转换
* `audioVisualization.py`: 提供了一系列功能，来把结果生成友好的和有代表性的图表

## 3.特征抽取

### 简介

音频特征抽取方法分为2类：短期时长的特征抽取及中期时长的特征抽取

* 短期时长的特征抽取：`stFeatureExtraction()`方法将音频信号拆分成短期的片段/元组，然后计算每个片段/元组的特征，最终生成整段音频的特征向量的序列。

* 中期时长的特征抽取：在很多情况下，一段信号需要被表示为提取出的短期片段的特征统计值，`mtFeatureExtraction()`则解决了这一问题，它根据整段音频的短期片段的特征向量的序列，计算了一些统计值，如均值、标准差等。


文件：`audioFeatureExtraction.py`

#### 短期时长特征抽取

核心方法：
`stFeatureExtraction()`


```python
def stFeatureExtraction(signal, fs, win, step):
    """
    This function implements the shor-term windowing process. For each short-term window a set of features is extracted.
    This results to a sequence of feature vectors, stored in a numpy matrix.

    ARGUMENTS
        signal:       the input signal samples
        fs:           the sampling freq (in Hz)
        win:          the short-term window size (in samples)
        step:         the short-term window step (in samples)
    RETURNS
        st_features:   a numpy array (n_feats x numOfShortTermWindows)
    """
```

参数：
> signal：音频的样本，注：格式为一维数组
> fs：采样频率
> win：计算窗口
> step：计算步长

方法会返回一个34行n列的数组，其中每行是一类特征向量，共34类特征。n是样本数/步长，即`len(signal)/step`


#### 中期时长特征抽取

核心方法：
`mtFeatureExtraction(signal, fs, mt_win, mt_step, st_win, st_step)`


### 单文件特征抽取-输出到文件

核心方法：
`mtFeatureExtractionToFile()`


```python
def mtFeatureExtractionToFile(fileName, midTermSize, midTermStep, shortTermSize, shortTermStep, outPutFile, storeStFeatures=False, storeToCSV=False, PLOT=False):
    """
    This function is used as a wrapper to:
    a) read the content of a WAV file
    b) perform mid-term feature extraction on that signal
    c) write the mid-term feature sequences to a numpy file
    """
```

此方法会返回2个文件：`{defined_name}.csv`和`{defined_name}_st.csv`，分别存储了中期时长和短期时长的特征数据。
* 短期时长的特征矩阵：每一个特征序列都存储在不同的列里，即列是特征数据（34列），行是时间窗口。
* 中期时长的特征矩阵：列是统计过的特征数据（68列，前34列是均值，后34列是标准差），行是时间窗口

同样，也可以返回2个numpy支持的文件.npy。


### 批量文件特征抽取-输出到文件

核心方法：
`mtFeatureExtractionToFileDir(dirName, midTermSize, midTermStep, shortTermSize, shortTermStep, storeStFeatures=False, storeToCSV=False, PLOT=False)`

与上面的方法类似。

注意：上面2个特征提取的方法，因为没有进行长期时长的平均，因此生成的都是特征矩阵，而非一个特征向量。而`dirWavFeatureExtraction()`和`dirsWavFeatureExtraction()`方法执行了这一步骤。


### 声谱及色谱可视化

核心方法：
`stSpectogram()` 和 `stChromagram()`



### 节拍提取

节拍感应在音乐信息检索领域，是一项非常重要的任务。本框架提供了一个基础方法来估算一段音乐每分钟的节拍数。`beatExtraction()`方法实现了这一功能。此方法有2个参数：a)短期时长的特征矩阵，b)窗口步长。


注意：当音频时长超过大于1分钟后，此方法的可视化非常耗时。
注：本功能仅适用在长期时长的分析方法。因此，执行长期平均的功能，如`dirWavFeatureExtraction()`，可以选择计算BPM作为一类特征。



## 4.分类与回归

### 4.1分类

`audioTrainTest.py`实现了基于以下算法的分类器：
* k Nearest Neighbor kNN (implemented in the library itself)
* Support Vector Machines
* Random forests
* Extra trees
* Gradient boosting

`audioTrainTest.py`中包含以下方法：
* `classifierWrapper()`:分类未知的样本
* `randSplitFeatures()`:将实验样本随机拆分成训练集和测试集，用于交叉验证
* `trainKNN()`, `trainSVM()`, `trainSVM_RBF()`, `trainExtraTrees()`, `trainRandomForest()` and `trainGradientBoosting()`: 基于不同算法的训练模型
* `normalizeFeatures()`:  将数据集进行标准化，进行0平均和归一化处理
* `load<methodName>Model()`: 从文件中加载分类模型

#### 训练分类器

核心方法：
`featureAndTrain(listOfDirs, mtWin, mtStep, stWin, stStep, classifierType, modelName, computeBEAT)`

```python
def featureAndTrain(list_of_dirs, mt_win, mt_step, st_win, st_step,
                    classifier_type, model_name,
                    compute_beat=False, perTrain=0.90):
    '''
    This function is used as a wrapper to segment-based audio feature extraction and classifier training.
    ARGUMENTS:
        list_of_dirs:        list of paths of directories. Each directory contains a signle audio class whose samples are stored in seperate WAV files.
        mt_win, mt_step:        mid-term window length and step
        st_win, st_step:        short-term window and step
        classifier_type:        "svm" or "knn" or "randomforest" or "gradientboosting" or "extratrees"
        model_name:        name of the model to be saved
    RETURNS:
        None. Resulting classifier along with the respective model parameters are saved on files.
    '''
```

参数：
> listOfDirs: 文件夹路径，格式为数组
> mtWin, mtStep: 中等时长的窗口及步长
> stWin, stStep: 短期时长的窗口及步长
> classifierType: 分类算法，"svm" or "knn" or "randomforest" or "gradientboosting" ……
> modelName: 保存的模型名称
> computeBEAT: 是否计算节拍

方法会返回一个分类器，并存到文件中。


#### 单文件分类

核心方法：
`fileClassification(inputFile, modelName, modelType)`


```
# 加载模型
[classifier, MEAN, STD,...] = load_model(model_name)
# 读取文件
[Fs, x] = audioBasicIO.readAudioFile(inputFile)
# 转换为单声道
x = audioBasicIO.stereo2mono(x)
# 特征抽取
[mt_features, s, _] = aF.mtFeatureExtraction(x, Fs, mt_win * Fs, mt_step * Fs, round(Fs * st_win), round(Fs * st_step))
# 归一化处理
mt_features = mt_features.mean(axis=1)        # long term averaging of mid-term statistics
# 标准化
curFV = (mt_features - MEAN) / STD                # normalization
# 执行分类
[Result, P] = classifierWrapper(classifier, model_type, curFV)    # classification
return Result, P, classNames
```

参数：
> inputFile: 分类的文件，wav或者mp3格式都可以
> modelName: 模型文件名
> modelType: 模型使用的算法


### 4.2回归

回归也很重要，回归需要估计出一个表示程度的值，而不像分类那样划分到某个类别。典型的场景是情感分析。

不同于分类方法（按文件夹对训练集进行分类），回归时的训练集都放在同一个文件夹中，然后在此文件夹下的csv文件中存放标注的信息。csv的文件名表示其分类，文件中有2列，一列是wav的文件名，一列是标注值。如果有多个csv文件，表示训练多个csv文件

`featureAndTrainRegression()`中的主要方法：
* dirsWavFeatureExtraction(): 特征抽取
* evaluateRegression(): 抽取一个优化后的回归模型


#### 训练回归模型

核心方法：
`featureAndTrainRegression(dir_name, mt_win, mt_step, st_win, st_step, model_type, model_name, compute_beat=False)`


```python
def featureAndTrainRegression(dir_name, mt_win, mt_step, st_win, st_step,
                              model_type, model_name, compute_beat=False):
    '''
    This function is used as a wrapper to segment-based audio feature extraction and classifier training.
    ARGUMENTS:
        dir_name:        path of directory containing the WAV files and Regression CSVs
        mt_win, mt_step:        mid-term window length and step
        st_win, st_step:        short-term window and step
        model_type:        "svm" or "knn" or "randomforest"
        model_name:        name of the model to be saved
    RETURNS:
        None. Resulting regression model along with the respective model parameters are saved on files.
    '''
```

参数：
> dir_name: 文件夹路径
> mt_win, mt_step: 中等时长的窗口及步长
> st_win, st_step: 短期时长的窗口及步长
> model_type, model_name: 模型算法类型，要存储的模型文件名（可带路径）
> compute_beat=False: 是否计算节拍


#### 单文件回归

核心方法：
`fileRegression(inputFile, model_name, model_type)`


```
# 加载模型
regression_models = glob.glob(model_name + "_*")
[_, _, _, mt_win, mt_step, st_win, st_step, compute_beat] = load_model(regression_models[0], True)

# 读取文件
[Fs, x] = audioBasicIO.readAudioFile(inputFile)
# 转换为单声道
x = audioBasicIO.stereo2mono(x)
# 特征抽取
[mt_features, s, _] = aF.mtFeatureExtraction(x, Fs, mt_win * Fs, mt_step * Fs, round(Fs * st_win), round(Fs * st_step))
# 归一化处理
mt_features = mt_features.mean(axis=1)        # long term averaging of mid-term statistics

# 执行回归计算(多个模型)
R = []
for ir, r in enumerate(regression_models):
    if not os.path.isfile(r):
        print("fileClassification: input model_name not found!")
        return (-1, -1, -1)
    if model_type == 'svm' or model_type == "svm_rbf" \
            or model_type == 'randomforest':
        [model, MEAN, STD, mt_win, mt_step, st_win, st_step, compute_beat] = \
            load_model(r, True)
    # 标准化
    curFV = (mt_features - MEAN) / STD
    R.append(regressionWrapper(model, model_type, curFV))    # classification

 return R, regression_names
```

参数：
> inputFile: 分类的文件，wav或者mp3格式都可以
> modelName: 模型文件名
> modelType: 模型使用的算法

## 5.分割

音频分割是音频分析过程中非常重要的处理环节，其目的是把连续的音频信号分割成均匀的或者“同类”的音频片段。“同类”的概念很难定义，所以此框架分了2类。一类是监督的，一类是非监督的。

* 监督：
可以通过分类器将固定大小的片段划分为预定义的不同类别，也可以使用HMM方法实现分割
* 非监督：
通过聚类进行分割，如：静音识别及移除，发声者的数字化，音频摘要

### 固定大小的分割与分类

使用已有的分类器将一段音频分割成固定大小的片段，会产生一个分类标签的序列来描述整段音频的特征。

核心方法：
`mtFileClassification(input_file, model_name, model_type, plot_results=False, gt_file="")`

此功能：
* 首先将音频拆分成中等时长的片段，并抽取这些片段的特征，
* 然后使用预先训练好的模型对每个片段进行分类，
* 然后对相邻的且为相同类别的片段进行合并，
* 最后将结果可视化。


```python
def mtFileClassification(input_file, model_name, model_type,
                         plot_results=False, gt_file=""):
    '''
    This function performs mid-term classification of an audio stream.
    Towards this end, supervised knowledge is used, i.e. a pre-trained classifier.
    ARGUMENTS:
        - input_file:        path of the input WAV file
        - model_name:        name of the classification model
        - model_type:        svm or knn depending on the classifier type
        - plot_results:      True if results are to be plotted using
                             matplotlib along with a set of statistics

    RETURNS:
          - segs:           a sequence of segment's endpoints: segs[i] is the
                            endpoint of the i-th segment (in seconds)
          - classes:        a sequence of class flags: class[i] is the
                            class ID of the i-th segment
    '''
```

参数：
> input_file: 要分段的音频文件
> model_name, model_type: 预定义的模型名称，模型算法类型（svm or knn）
> plot_results: 是否绘制结果（True or False）
> gt_file: 结果校验文件（数据标注文件）

返回结果:
> flags_ind: 片段类型的标记（标记列表class_names_gt的索引），片段数按训练模型时mtWin的值分割
> class_names_gt: 标记列表
> acc: 准确率
> cm: 各标记的统计



### 基于HMM的分割与分类

HMMs基于监督算法，因此HMM模型所需的转换和先验矩阵需要先被训练出来。为了这一目的，可以使用`trainHMM_fromFile()`或`trainHMM_fromFile()`来训练一个HMM模型，其中`trainHMM_fromFile()`通过1个标注过的文件来训练，`trainHMM_fromDir()`可以使用放在某个指定目录里的多个文件来训练。两种方法中 文件的标注通过.segments格式的文件来实现。

一旦模型完成训练，可以使用`hmmSegmentation()`方法来应用HMM模型，为了评估最合适的分类序列，会分别给出中等时长特征向量。 注意：与固定长度的分割方法一样，`hmmSegmentation()`方法使用`plotSegmentationResults()`方法来将分片结果和评估结果可视化。

注意：如果是短期时长的事件，如阅读单词，那么在训练模型时，需要用更小的窗口及步长（mt_win, mt_step）。

核心方法：
1. `trainHMM_fromFile(wav_file, gt_file, hmm_model_name, mt_win, mt_step)`


```python
def trainHMM_fromFile(wav_file, gt_file, hmm_model_name, mt_win, mt_step):
    '''
    This function trains a HMM model for segmentation-classification using a single annotated audio file
    ARGUMENTS:
     - wav_file:        the path of the audio filename
     - gt_file:         the path of the ground truth filename
                       (a csv file of the form <segment start in seconds>,<segment end in seconds>,<segment label> in each row
     - hmm_model_name:   the name of the HMM model to be stored
     - mt_win:          mid-term window size
     - mt_step:         mid-term window step
    RETURNS:
     - hmm:            an object to the resulting HMM
     - class_names:     a list of class_names

    After training, hmm, class_names, along with the mt_win and mt_step values are stored in the hmm_model_name file
    '''
```

参数：
> wav_file: 用于训练的音频文件
> gt_file: 用于训练的音频标注文件
> hmm_model_name: 要生成的模型名称
> mt_win, mt_step: 中等时长的窗口及步长


2. `hmmSegmentation(wav_file_name, hmm_model_name, plot_res=False, gt_file_name="")`

参数及返回 类似于`mtFileClassification()`


注1：hmmRadioSM是一个训练好的模型，来给音乐和讲话进行分类。
注2：`evaluateSegmentationClassificationDir()`用来评估不同分割方法/模型的效果


### 静音移除/有声检测

`audioSegmentation.py`中的`silenceRemoval()`方法将连续的音频拆分为独立的事件片段，即静默的信号都被移除掉了。
其实现主要通过一个半监督方法：首先训练一个SVM模型来分辨（短期时长的）高能信号与低能信号，使用其中10%的高能片段和10%的低能片段来作为训练集。然后对整段音频应用这一SVM训练模型，并使用动态的阈值来判断动态的片段。

核心方法：`silenceRemoval(x, fs, st_win, st_step, smoothWindow=0.5, weight=0.5, plot=False)`


```python
def silenceRemoval(x, fs, st_win, st_step, smoothWindow=0.5, weight=0.5, plot=False):
    '''
    Event Detection (silence removal)
    ARGUMENTS:
         - x:                the input audio signal
         - fs:               sampling freq
         - st_win, st_step:    window size and step in seconds
         - smoothWindow:     (optinal) smooth window (in seconds)
         - weight:           (optinal) weight factor (0 < weight < 1) the higher, the more strict
         - plot:             (optinal) True if results are to be plotted
    RETURNS:
         - seg_limits:    list of segment limits in seconds (e.g [[0.1, 0.9], [1.4, 3.0]] means that
                    the resulting segments are (0.1 - 0.9) seconds and (1.4, 3.0) seconds
    '''
```

参数：
> x: 输入的音频（数字化的）
> fs: 采样频率
> st_win, st_step: 短期时长的窗口及步长
> smoothWindow=0.5: 平滑窗口（单位秒）
> weight=0.5: 决策阈值（越高越严格）
> plot=False: 是否可视化结果

返回结果seg_limits是一个数组，表示非静音（有声）片段的起止时间。

根据音频性质的不同，也应该使用不同的平滑窗口和决策阈值。上述的样本中，声音是非常稀疏的。对于持续的讲话，应该使用更短（值更小）的平滑窗口和更严格的（值更大）的决策阈值。


### 演讲者数字化/演讲者识别

演讲者数字化能够自动回答：“什么时间是谁在说话”的问题。

通常，演讲者数字化会执行以下一系列的算法步骤：
* 特征抽取（短期时长和中期时长）：对于中期时长的片段，会使用MFCCs特征的均值和标准差，以及性别的判断来作为综合的特征。（性别的判断使用已经训练好的knnSpeakerFemaleMale模型）
* FLsD步骤（可选）：这步中使用FLsD方法，根据中期时长的统计特征向量，获得了近似最佳的演讲者预测结果
* 聚类：使用k-means聚类方法。如果演讲者的数量不是事先确定的，那么聚类算法会重复执行，计算出一些不同的演讲者数量，然后使用Silhouette width（轮廓宽度）标准来找到最优解。参考：  [https://en.wikipedia.org/wiki/Silhouette_(clustering)](https://en.wikipedia.org/wiki/Silhouette_(clustering))
* 平滑：在抽取出的类别ID上进行中值过滤 并进行 一个维特比平滑


核心方法：`speakerDiarization(filename, n_speakers, mt_size=2.0, mt_step=0.2, st_win=0.05, lda_dim=35, plot_res=False)`


```python
def speakerDiarization(filename, n_speakers, mt_size=2.0, mt_step=0.2,
                       st_win=0.05, lda_dim=35, plot_res=False):
    '''
    ARGUMENTS:
        - filename:        the name of the WAV file to be analyzed
        - n_speakers    the number of speakers (clusters) in the recording (<=0 for unknown)
        - mt_size (opt)     mid-term window size
        - mt_step (opt)     mid-term window step
        - st_win  (opt)     short-term window size
        - lda_dim (opt)     LDA dimension (0 for no LDA)
        - plot_res     (opt)   0 for not plotting the results 1 for plottingy
    '''
```

参数：
> filename: 输入的音频
> n_speakers: 演讲者人数
> mt_size=2.0, mt_step=0.2: 中期时长的窗口及步长
> st_win=0.05: 短期时长的窗口
> lda_dim=35: LDA维数
> plot_res=False: 是否结果可视化



### 音频摘要

音频摘要是在音乐信息检索领域的一类重要应用，它主要用来检测或分析一段音乐中最具代表性的部分。

输入一段音频，`musicThumbnailing()`方法会生成2片摘要，摘要长度由thumb_size参数定义。

核心方法：`musicThumbnailing(x, fs, short_term_size=1.0, short_term_step=0.5, thumb_size=10.0, limit_1 = 0, limit_2 = 1)`



```python
def musicThumbnailing(x, fs, short_term_size=1.0, short_term_step=0.5,
                      thumb_size=10.0, limit_1 = 0, limit_2 = 1):
    '''
    This function detects instances of the most representative part of a
    music recording, also called "music thumbnails".
    A technique similar to the one proposed in [1], however a wider set of
    audio features is used instead of chroma features.
    In particular the following steps are followed:
     - Extract short-term audio features. Typical short-term window size: 1 second
     - Compute the self-silimarity matrix, i.e. all pairwise similarities between feature vectors
     - Apply a diagonal mask is as a moving average filter on the values of the self-similarty matrix.
       The size of the mask is equal to the desirable thumbnail length.
     - Find the position of the maximum value of the new (filtered) self-similarity matrix.
       The audio segments that correspond to the diagonial around that position are the selected thumbnails


    ARGUMENTS:
     - x:            input signal
     - fs:            sampling frequency
     - short_term_size:     window size (in seconds)
     - short_term_step:    window step (in seconds)
     - thumb_size:    desider thumbnail size (in seconds)

    RETURNS:
     - A1:            beginning of 1st thumbnail (in seconds)
     - A2:            ending of 1st thumbnail (in seconds)
     - B1:            beginning of 2nd thumbnail (in seconds)
     - B2:            ending of 2nd thumbnail (in seconds)

    USAGE EXAMPLE:
       import audioFeatureExtraction as aF
     [fs, x] = basicIO.readAudioFile(input_file)
     [A1, A2, B1, B2] = musicThumbnailing(x, fs)

    [1] Bartsch, M. A., & Wakefield, G. H. (2005). Audio thumbnailing
    of popular music using chroma-based representations.
    Multimedia, IEEE Transactions on, 7(1), 96-104.
    '''
```

参数：
> x, fs: 输入的音频信号及采样频率
> short_term_size=1.0, short_term_step=0.5:  短期时长的计算窗口及步长（单位秒）
> thumb_size=10.0: 所需的摘要的时长（单位秒）
> limit_1 = 0, limit_2 = 1: ？

返回：
>A1, A2: 第一段摘要的起止时间
>B1, B2: 第二段摘要的起止时间
>S: 自相似矩阵


## 6. 数据可视化

这个库使用d3js框架可以将音频的相似之处进行可视化。主要方法是`audioVisualization.py`中的`dirWavFeatureExtraction()`，此方法：
1. 先使用`dirWavFeatureExtraction()`对文件夹中的每个音频抽取长期时长的特征，
2. 然后使用PCA或者LDA算法进行降维。由于LDA是监督算法，即需要进行训练，所以需要对输入的文件进行标注。可以通过文件名进行标注，使用`---`来分割，前面是分组信息，后面是文件名。
3. 降维之后，计算相似度矩阵，对这一相似度矩阵进行阈值切割
4. 生成和弦图。不同的颜色的边缘代表不同的种类，边缘之间的连线代表内容相似度。

![sss-w500](https://ooo.0o0.ooo/2019/02/20/5c6d05ea66416.jpg)



## 7. 音频录制相关功能

`audioAnalysisRecordAlsa.py`库中提供了一些音频分析的基础功能。然而，它依赖于`alsa-audio`python库，这个库只在Linux系统可用。

### 录音成固定大小的音频片段

`recordAudioSegments(RecordPath, BLOCKSIZE)`: 能录制固定大小的音频，并将它们存储到文件夹中。


### 实时音频录制及分类

`recordAnalyzeAudio(duration, outputWavFile, midTermBufferSizeSec, modelName, modelType)`



```python
def recordAnalyzeAudio(duration, outputWavFile, midTermBufferSizeSec, modelName, modelType):
	'''
	recordAnalyzeAudio(duration, outputWavFile, midTermBufferSizeSec, modelName, modelType)

	This function is used to record and analyze audio segments, in a fix window basis.

	ARGUMENTS:
	- duration			total recording duration
	- outputWavFile			path of the output WAV file
	- midTermBufferSizeSec		(fix)segment length in seconds
	- modelName			classification model name
	- modelType			classification model type

	'''
```

参数：
> duration: 总录音的时长
> outputWavFile: 输出的路径及文件名
> midTermBufferSizeSec: 要分类的分段的时长（单位s）
> modelName, modelType: 模型名称和模型算法类型


## 8. 其他方法

* `convertDirMP3ToWav(dirName, Fs, nC, useMp3TagsAsName = False)`: 把mp3
转成wav
* `audioBasicIO.readAudioFile(path)`: 读取文件，转化为信号
* `audioBasicIO.stereo2mono(x)`: 信号转为单声道信号

---

