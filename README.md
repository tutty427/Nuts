# Nuts
自然语言处理（Natural Language Processing，NLP）常见任务（主要包括文本分类，序列标注，自动问答等）解决方案试验田

## 文本分类（Text Classification）
将一段文本（可以是词、句子、文章）分门别类，打上预定义好的一个或多个标签，是非常常见的一类应用需求，如：

* 垃圾邮件分类：典型的二元分类问题，常被拿来举例
* 网页分类：包括新闻资讯，电商商品，微信公众号文章以及普通 web 网页，通常是长文本，信息较为充足，但噪声大，类目较多
* query 分类：搜索引擎场景下核心处理模块，通常是短文本，信息不足是最大挑战
* 情感分类：处理文本通常是偏口语化的评论，粒度包括词语级、属性级、句子级和篇章级，类别个数通常较少（褒/贬/中性，喜/怒/悲/恐/惊）
* 意图识别/分类：聊天机器人场景下核心处理模块

### 数据集
本项目中，我们将针对如下数据集，详细对比多种不同的传统机器学习和深度学习解决方案，如 LR，MaxEnt，FastText，TextCNN，TextRNN，Attention Model，等等，希望可以找到普适最优的算法模型或技术思路，积累可复用的工具集。

* 淘宝电商商品分类：https://tianchi.aliyun.com/datalab/dataSet.htm?spm=5176.100073.888.25.4830d926tXuyxj&id=18 ，阿里巴巴在天池平台上开放的一个商品和类目的数据集，涵盖了 1500w 左右淘宝行业商品库，类目数将近 2,000 个。
* 新闻资讯分类（20 Newsgroups）：http://archive.ics.uci.edu/ml/datasets/Twenty+Newsgroups ，共有 18K+ 篇新闻文章，20 个类别。
* IMDB 电影评论情感分类：http://ai.stanford.edu/~amaas/data/sentiment/ ，从 imdb.com 网站收集的电影评论，区分积极或消极的情绪。

### 分类策略

### 评估分析

## 序列标注（Sequence Labelling）
序列标注就是为给定的一维线性输入序列的每个元素，打上标签集合中的某个标签的过程，其本质上是对线性序列中每个元素根据上下文内容进行分类的问题，是结构化预测的一种特例。常见的任务有：

* 中文分词：为汉字串
* 词性标注：
* 命名实体识别：
* 语义角色标注：
* 实体关系抽取：

最常用的解决序列标注问题的模型是 HMM，MEMM，CRF，Structured Perceptron/SVM 等，尤其是 CRF 和 Structured Perceptron，是最主流的方法。近年来，基于 RNN 的深度学习方法，尤其是 LSTM，BiLSTM，LSTM+CRF，BiLSTM+CRF 取得了更优的效果，基本成了解决序列标注问题的标配方案。

### 数据集
本项目中，我们将针对如下数据集，主要对比 CRF，Structured Perceptron 和 RNN 三种解决方案。

* 中文分词：XXX
* 命名实体识别：XXX

### 分类策略

### 评估分析

## 自动问答（Question Answering）
