﻿每个项目已经提供了相应的数据集，和详细的注释。 

#### 数据集
1. 综合类中文词库.xlsx： 包含了中文词，当做词典来用 （用于PART1)
2. dev-v2.0.json: 这个数据包含了问题和答案的pair， 但是以JSON格式存在，需要编写parser来提取出里面的问题和答案。 (用于PART2) 
3. glove.6B: 这个文件需要从网上下载，下载地址为：https://nlp.stanford.edu/projects/glove/， 请使用d=100的词向量 (用于PART3)

#### 环境：
Python 3 (必须要使用Python 3)

#### 任务描述

#### 分词工具编写
- 利用枚举法来实现分词，也就是首先把所有可能的分词结果列出来，然后通过UNIGRAM模型来选择最好的分词结构（这部分的难点在于怎么生成所有的可能的分词结果）
- 利用维特比算法来实现分词。这部分首先需要创建一个有向图，然后根据维特比算法来计算出最好的分词结果。这部分里的创建有向图和维特比部分需要一定的思考。 

#### 简单的问答系统编写
- 文本的读取： 从JSON文件里读数据，并把文本写到问题变量和答案变量中（list）
- 文本的预处理： 需要对原始文本做预处理操作，包括一些词的过滤
- 文本的表示： 把文本转换成tf-idf格式/词向量，句子向量
- 文本相似度计算： 利用余弦相似度来计算文本之间的相似度
- 倒排列表：通过倒排列表来加快文档的检索

#### 知识抽取
- 详见notebook

#### seq2seq_Att
参考知乎：https://zhuanlan.zhihu.com/p/81761891




