# RAG-with-Gemma-hosted-on-HuggingFace-and-Weaviate-in-DSPy
# 项目简介
## 概述
本项目简要介绍了如何使用 DSPy 构建一个简单的 RAG 管道，且利用了托管在 Hugging Face 上的 Gemma LLM模型 和 Weaviate 向量数据库。
## 时间
2024.09.06-2024.09.07
## kaggle地址
[RAG with Gemma hosted on HuggingFace and Weaviate in DSPy](https://www.kaggle.com/code/chenxucool/rag-with-gemma-on-hf-and-weaviate-in-dspy)

## 技术博客地址
[我的第2个AI项目-RAG with Gemma hosted on HuggingFace and Weaviate in DSPy](https://blog.csdn.net/weixin_43221845/article/details/141963587?csdn_share_tail=%7B%22type%22:%22blog%22,%22rType%22:%22article%22,%22rId%22:%22141963587%22,%22source%22:%22weixin_43221845%22%7D)

## 主要工作和收获
- 用 Weaviate 向量数据库来构建检索模型从而增强生成。
- 使用 DSPy 构建一个简单的 RAG 管道来增强生成。
- 使用少样本学习（Few-Shot Learning）来优化 RAG 模型 的问答生成能力。
- 掌握了如何使用 Hugging Face 上的LLM模型，比如 Gemma。
- 修复了一个版本兼容bug。

## 技术栈
- RAG，DSPy，Weaviate，Hugging Face，Gemma，Few-Shot Learning
##  数据集
meta-kaggle
## 模型表现
**问题**：Which Kaggle competition should I look at to learn more about recommender systems in e-commerce?
**答案（生成**）：
 - 未使用RAG的生成
答案较长，就不贴了，可以查看kaggle代码日志。结论是 Gemma 无法在没有额外上下文的情况下回答示例查询。
 - 使用未优化的RAG的生成
 

> The [1] competition is a good place to start learning about recommender systems in e-commerce. By analyzing the data provided in the competition, we can gain a better understanding of how to build a

效果不太理想



 - 使用少样本学习优化的RAG的生成

> You might be interested in the JPX Tokyo Stock Exchange Prediction or Jane Street Market Prediction or Ubiquant Market Prediction competition.

达到了预期效果，和少样本学习的例子格式完全一致。
