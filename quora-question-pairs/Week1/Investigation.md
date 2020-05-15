Week1——Investigation

By Xyao

Student Number ：20200116027

# 项目简介

Kaggle上2017年的Quora比赛（Text Matching）

数据集：Quora Question Pairs

目的：判断两个问题是否在表达相同的意思。

所以，项目要点在于文本相似性匹配或者说如何度量两个文本之间的相似度（一个问题可以看做一个文本）。

如今Quora Question Pairs数据集也是经常用于评价NLP模型在文本匹配任务上的性能。

# 调研情况

近年来，NLP领域越来越火热，涌现出大量具有代表性的模型。而文本匹配作为业界许多下游任务的基础，得到了学术界的广泛关注与重视。

在Quora Question Pairs数据集上获得较好表现的模型如下：

|   Method    |  Acc  |                            Paper                             | Code                                                         |
| :---------: | :---: | :----------------------------------------------------------: | ------------------------------------------------------------ |
|   MT-DNN    | 89.6  | [Multi-Task Deep Neural Networks for Natural Language Understanding](https://paperswithcode.com/paper/multi-task-deep-neural-networks-for-natural) | https://github.com/namisan/mt-dnn                            |
|     SAN     | 89.4  | [Stochastic Answer Networks for Natural Language Inference](https://arxiv.org/pdf/1804.07888v2.pdf) | https://github.com/kevinduh/san_mrc                          |
|     RE2     | 89.2  | [ Simple and Effective Text Matching with Richer Alignment Features](https://paperswithcode.com/paper/simple-and-effective-text-matching-with) | https://github.com/alibaba-edu/simple-effective-text-matching |
|    CSRAN    | 89.2  | [Co-Stack Residual Affinity Networks with Multi-level Attention Refinement for Matching Text Sequences](https://arxiv.org/abs/1810.02938v1) |                                                              |
|    MwAN     | 89.12 | [Multiway Attention Networks for Modeling Sentence Pairs](https://www.ijcai.org/Proceedings/2018/0613.pdf) | https://github.com/zsweet/zsw_AI_model                       |
|    DIIN     | 89.06 | [ Natural Language Inference over Interaction Space](https://paperswithcode.com/paper/natural-language-inference-over-interaction-1) | https://github.com/YichenGong/Densely-Interactive-Inference-Network |
|    MSEM     | 88.86 | [Multi-task Sentence Encoding Model for Semantic Retrieval in Question Answering Systems](https://paperswithcode.com/paper/multi-task-sentence-encoding-model-for) |                                                              |
| Bi-CAS-LSTM | 88.6  | [Cell-aware Stacked LSTMs for Modeling Sentences](https://paperswithcode.com/paper/cell-aware-stacked-lstms-for-modeling) |                                                              |
|  pt-DecAtt  | 88.40 | [ Neural Paraphrase Identification of Questions with Noisy Pretraining](https://paperswithcode.com/paper/neural-paraphrase-identification-of-questions) |                                                              |
|    BiMPM    | 88.17 | [Bilateral Multi-Perspective Matching for Natural Language Sentences](https://paperswithcode.com/paper/bilateral-multi-perspective-matching-for) | https://github.com/zhiguowang/BiMPM                          |
|   GenSen    | 87.01 | [Learning General Purpose Distributed Sentence Representations via Large Scale Multi-task Learning](https://paperswithcode.com/paper/learning-general-purpose-distributed-sentence) | https://github.com/facebookresearch/InferSent                |
|  SpanBERT   | 71.9  | [SpanBERT: Improving Pre-training by Representing and Predicting Spans](https://paperswithcode.com/paper/spanbert-improving-pre-training-by) | https://github.com/facebookresearch/SpanBERT                 |
|  TinyBERT   | 71.3  | [TinyBERT: Distilling BERT for Natural Language Understanding](https://paperswithcode.com/paper/190910351) | https://github.com/google-research/electra                   |
|    ERNIE    | 71.2  | [ERNIE: Enhanced Language Representation with Informative Entities](https://paperswithcode.com/paper/ernie-enhanced-language-representation-with) | https://github.com/thunlp/ERNIE                              |

此外，还有一些其他在文本匹配上有着出色表现的模型（论文中没有基于Quora做实验，就单独拿出来），如：

- [Text Matching as Image Recognition](https://arxiv.org/pdf/1602.06359v1.pdf)，Code地址：https://github.com/NTMC-Community/MatchZoo
- [Learning to Rank Short Text Pairs with Convolutional Deep Neural Networks](https://sci-hub.im/https://dl.acm.org/doi/abs/10.1145/2766462.2767738)，Code地址：暂无

上面这两篇文章都有在模型中加入卷积神经网络，且取得了较好的效果。

