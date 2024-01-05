# **Awesome Text2SQL**🎉🎉🎉


[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/eosphoros-ai/Awesome-Text2SQL/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)


[**English**](README.md) | **中文版**

这里收集了针对大型语言模型、Text2SQL、[Text2DSL](Text2DSL.md)、 [Text2API](Text2API.md)、 [Text2Vis](Text2Vis.md) 等的精选教程和资源。

## 🌱 如何贡献
我们热烈欢迎大家的贡献，无论您是发现拼写错误、错误、有建议，还是想要分享与LLM+Text2SQL相关的资源。有关如何贡献的详细指南，请参阅我们的 [CONTRIBUTING.md](CONTRIBUTING.md) 文件。

## 🔔 排行榜

|      |                              [WikiSQL](https://github.com/salesforce/WikiSQL#leaderboard)                               |                [Spider](https://yale-lily.github.io/spider)<br/>Exact Match(EM)                 |              [Spider](https://yale-lily.github.io/spider)<br/>Exact Execution(EX)               |    [BIRD](https://bird-bench.github.io/)<br/>Valid Efficiency Score (VES)     |       [BIRD](https://bird-bench.github.io/)<br/>Execution Accuracy (EX)        |
|:----:|:-----------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:------------------------------------------------------------------------------:|
| 🏆1  |             **93.0** <br/>(2021/05-[SeaD+Execution-Guided Decoding](https://arxiv.org/pdf/2105.07911.pdf))              |                                **81.5** <br/>(2023/11-MiniSeek)                                 |                                **91.2** <br/>(2023/11-MiniSeek)                                 |                   **67.68** <br/>(2023/11-MAC-SQL + GPT-4)                    | **60.71** <br/>(2023/11-[Dubo-SQL-v1](https://dubo.gg/posts/bird-benchmarks/)) |
| 🥈2  |               92.7 <br/>(2021/03-[SDSQL+Execution-Guided Decoding](https://arxiv.org/pdf/2103.04399.pdf))               |         74.0 <br/>(2022/09-[Graphix-3B + PICARD](https://arxiv.org/pdf/2301.07507.pdf))         | 86.6 <br/>(2023/08-[DAIL-SQL + GPT-4 + Self-Consistency](https://arxiv.org/pdf/2308.15363.pdf)) |                      64.22 <br/>(2023/10-SFT CodeS-15B)                       |                       60.37 <br/>(2023/10-SFT CodeS-15B)                       |
| 🥉3  |        92.5 <br/>(2020/11-[IE-SQL+Execution-Guided Decoding](https://aclanthology.org/2020.emnlp-main.563.pdf))         |                               73.9 <br/>(2022/09-CatSQL + GraPPa)                               |          86.2 <br/>(2023/08-[DAIL-SQL + GPT-4](https://arxiv.org/pdf/2308.15363.pdf))           |                       63.62 <br/>(2023/10-SFT CodeS-7B)                       |                      59.59 <br/>(2023/11-MAC-SQL + GPT-4)                      |
|  4   |             92.2 <br/>(2020/03-[HydraNet+Execution-Guided Decoding](https://arxiv.org/pdf/2008.04759.pdf))              |            73.1 <br/>(2022/09-[SHiP + PICARD](https://arxiv.org/pdf/2212.08785.pdf))            |                      85.6 <br/>(2023/10-DPG-SQL + GPT-4 + Self-Correction)                      |  63.00 <br/>(2023/11-[Dubo-SQL-v1](https://dubo.gg/posts/bird-benchmarks/))   |                       59.25 <br/>(2023/10-SFT CodeS-7B)                        |
|  5   |              91.9 <br/>(2020/12-[BRIDGE+Execution-Guided Decoding](https://arxiv.org/pdf/2012.12627.pdf))               | 72.9 <br/>(2022/05-[G³R + LGESQL + ELECTRA](https://aclanthology.org/2023.findings-acl.23.pdf)) |           85.3 <br/>(2023/04-[DIN-SQL + GPT-4](https://arxiv.org/pdf/2304.11015.pdf))           | 61.95 <br/>(2023/08-[DAIL-SQL + GPT-4](https://arxiv.org/pdf/2308.15363.pdf)) | 57.41 <br/>(2023/11-[DAIL-SQL + GPT-4](https://arxiv.org/pdf/2308.15363.pdf))) |
|  6   |               91.8 <br/>(2019/08-[X-SQL+Execution-Guided Decoding](https://arxiv.org/pdf/1908.08113.pdf))               |                          72.4 <br/>(2022/08-RESDSQL+T5-1.1-lm100k-xl)                           |                    83.9 <br/>(2023/07-Hindsight Chain of Thought with GPT-4)                    |                          60.77 <br/>(2023/07-GPT-4)                           |  55.90 <br/>(2023/08-[DIN-SQL + GPT-4](https://arxiv.org/pdf/2304.11015.pdf))  |
|  7   |                            91.4 <br/>(2021/03-[SDSQL](https://arxiv.org/pdf/2103.04399.pdf))                            |                                    72.4 <br/>(2022/05-T5-SR)                                    |      82.3 <br/>(2023/06-[C3 + ChatGPT + Zero-Shot](https://arxiv.org/pdf/2307.07306.pdf))       | 59.44 <br/>(2023/08-[DIN-SQL + GPT-4](https://arxiv.org/pdf/2304.11015.pdf))  |                           54.89 <br/>(2023/07-GPT-4)                           |
|  8   |                           91.1 <br/>(2020/12-[BRIDGE](https://arxiv.org/pdf/2012.12627.pdf))                            |   72.2 <br/>(2022/12-[N-best List Rerankers + PICARD](https://arxiv.org/pdf/2210.10668.pdf))    |           80.8 <br/>(2023/07-Hindsight Chain of Thought with GPT-4 and Instructions)            |  56.56 <br/>(2023/03-[ChatGPT + CoT](https://arxiv.org/pdf/2305.03111.pdf))   |                         49.02 <br/>(2023/07-Claude-2)                          |
|  9   | 91.0 <br/>(2021/04-[Text2SQLGen + EG](https://www.semanticscholar.org/reader/b877233410484b2ff2add278105c53b6633d9d20)) |          72.1 <br/>(2021/09-[S²SQL + ELECTRA ](https://arxiv.org/pdf/2203.06958.pdf))           |         79.9 <br/>(2023/02-[RESDSQL-3B + NatSQ](https://arxiv.org/pdf/2302.05965.pdf))          |                         51.40 <br/>(2023/03-ChatGPT)                          |                         47.74 <br/>(2023/11-Open-SQL)                          |
|  10  |                        90.5 <br/>(2020/11-[SeqGenSQL+EG](https://arxiv.org/pdf/2011.03836.pdf))                         |         72.0 <br/>(2023/02-[RESDSQL-3B + NatSQL](https://arxiv.org/pdf/2302.05965.pdf))         |                                 78.5 <br/>(2022/11-SeaD + PQL)                                  |  49.69 <br/>(2023/03-[ChatGPT + CoT](https://arxiv.org/pdf/2305.03111.pdf))   |   40.08 <br/>(2023/03-[ChatGPT + CoT](https://arxiv.org/pdf/2305.03111.pdf))   |



## 📜 目录
- [**Awesome Text2SQL**🎉🎉🎉](#awesome-text2sql)
  - [🌱 如何贡献](#-如何贡献)
  - [📜 目录](#-目录)
  - [👋 简介](#-简介)
  - [📖 综述](#-综述)
  - [💬 经典模型](#-经典模型)
  - [🔥 基础模型](#-基础模型)
  - [💡 微调](#-微调)
  - [💪 数据集](#-数据集)
  - [🌈 评测指标](#-评测指标)
  - [🔧 实践项目](#-实践项目)
  - [🤝 友情链接](#-友情链接)


## 👋 简介
- Text-to-SQL（或者Text2SQL），顾名思义就是把文本转化为SQL语言，更学术一点的定义是：把数据库领域下的自然语言（Natural Language，NL）问题，转化为在关系型数据库中可以执行的结构化询语言（Structured Query Language，SQL），因此Text-to-SQL也可以被简写为NL2SQL。
  - 输入：自然语言问题，比如“*查询表t_user的相关信息，结果按id降序排序，只保留前10个数据*”
  - 输出：SQL，比如“*SELECT * FROM t_user ORDER BY id DESC LIMIT 10*”


## 📖 综述
- (2023-International Conference on Very Large Data Bases, VLDB, CCF-A）A survey on deep learning approaches for text-to-SQL [[paper](https://link.springer.com/article/10.1007/s00778-022-00776-8)]
- (2022-IEEE Transactions on Knowledge and Data Engineering, TKDE, CCF-A) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
- (2022-International Conference on Computational Linguistics, COLOING, CCF-B) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect [[paper](https://arxiv.org/pdf/2208.10099v1.pdf)]
- (2022-arXiv)Deep Learning Driven Natural Languages Text to SQL Query Conversion: A Survey [[paper](https://arxiv.org/pdf/2208.04415.pdf)]



## 💬 经典模型

- (2023-arXiv, None) **DBCᴏᴘɪʟᴏᴛ**: Scaling Natural Language Querying to Massive Databases
[[paper](https://arxiv.org/pdf/2312.03463.pdf)]
[[code](https://github.com/tshu-w/DBCopilot)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)
[![](https://img.shields.io/badge/Spider--Syn-blue)](https://arxiv.org/pdf/2106.01065.pdf)
[![](https://img.shields.io/badge/BIRD-red)](https://bird-bench.github.io/)

- (2023-arXiv, None) Text-to-SQL Empowered by Large Language Models: A Benchmark Evaluation
[[paper](https://arxiv.org/pdf/2308.15363v2.pdf)]
[[code](https://github.com/beachwang/dail-sql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)

- (2023-AAAI 2023, CCF-A) RESDSQL: Decoupling Schema Linking and Skeleton Parsing for Text-to-SQL
[[paper](https://arxiv.org/abs/2302.05965)]
[[code](https://github.com/RUCKBReasoning/RESDSQL)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)
[![](https://img.shields.io/badge/Spider--DK-blue)](https://arxiv.org/pdf/2109.05157.pdf)
[![](https://img.shields.io/badge/Spider--Syn-red)](https://arxiv.org/pdf/2106.01065.pdf)

- (2023-arXiv, None) Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs
[[paper](https://arxiv.org/pdf/2305.03111.pdf)]
[[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)]
[![](https://img.shields.io/badge/BIRD-green)](https://bird-bench.github.io/)

- (2023-arXiv, None) **DIN-SQL**: Decomposed In-Context Learning of Text-to-SQL with Self-Correction
[[paper](https://arxiv.org/pdf/2304.11015v2.pdf)]
[[code](https://github.com/mohammadrezapourreza/few-shot-nl2sql-with-prompting)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/WikiSQL-yellow)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2023-arXiv, None) A comprehensive evaluation of ChatGPT's zero-shot Text-to-SQL capability
[[paper](https://arxiv.org/pdf/2303.13547v1.pdf)]
[[code](https://github.com/THU-BPM/chatgpt-sql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)
[![](https://img.shields.io/badge/Spider--DK-blue)](https://arxiv.org/pdf/2109.05157.pdf)
[![](https://img.shields.io/badge/Spider--Syn-red)](https://arxiv.org/pdf/2106.01065.pdf)
[![](https://img.shields.io/badge/Spider--CG-organge)](https://arxiv.org/pdf/2205.02054.pdf)
[![](https://img.shields.io/badge/ADVETA-purple)](https://aclanthology.org/2022.acl-long.142.pdf)
[![](https://img.shields.io/badge/CSpider-cyan)](https://taolusi.github.io/CSpider-explorer/)
[![](https://img.shields.io/badge/DuSQL-lightgreen)](https://aclanthology.org/2020.emnlp-main.562.pdf)
[![](https://img.shields.io/badge/SParC-pink)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-gray)](https://arxiv.org/pdf/1909.05378.pdf)

- (2023-ICLR, CCF-A) Binding Language Models in Symbolic Languages
[[paper](https://arxiv.org/pdf/2210.02875v2.pdf)]
[[code](https://github.com/hkunlp/binder)]
[![](https://img.shields.io/badge/WIKITQ-green)](https://arxiv.org/pdf/1508.00305.pdf)
[![](https://img.shields.io/badge/TabFact-yellow)](https://arxiv.org/pdf/1909.02164.pdf)
[![](https://img.shields.io/badge/SOUALL-blue)](https://arxiv.org/pdf/2010.11246.pdf)

- (2023-SIGMOD, CCF-A) Few-shot Text-to-SQL Translation using Structure and Content Prompt Learning
[[paper](https://dl.acm.org/doi/abs/10.1145/3589292)]
[[code](https://github.com/ruc-datalab/SC-prompt)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)
[![](https://img.shields.io/badge/GenQuery-blue)](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=1c9df99cce1903d34c53025e86e72331bbfbe08f)

- (2023-ICASSP, CCF-B) **T5-SR**: A Unified Seq-to-Seq Decoding Strategy for Semantic Parsing
[[paper](https://arxiv.org/pdf/2306.08368v1.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)

- (2022-ACL, CCF-A) **S<sup>2</sup>SQL**: Injecting Syntax to Question-Schema Interaction Graph Encoder for Text-to-SQL Parsers
[[paper](https://aclanthology.org/2022.findings-acl.99.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)

- (2022-NAACL, CCF-B) **SeaD**: End-to-end Text-to-SQL Generation with Schema-aware Denoising
[[paper](https://arxiv.org/pdf/2105.07911v2.pdf)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)


- (2022-EMNLP, CCF-B) **STAR**: SQL Guided Pre-Training for Context-dependent Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/2210.11888v2.pdf)]
[[code](https://github.com/alibabaresearch/damo-convai)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2022-EMNLP, CCF-B) **RASAT**: Integrating Relational Structures into Pretrained Seq2Seq Model
for Text-to-SQL
[[paper](https://arxiv.org/pdf/2205.06983v2.pdf)]
[[code](https://github.com/LUMIA-group/rasat)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/SParC-yellow)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-blue)](https://arxiv.org/pdf/1909.05378.pdf)

- (2022-EMNLP, CCF-B) **CQR-SQL**: Conversational Question Reformulation Enhanced Context-Dependent Text-to-SQL Parsers
[[paper](https://arxiv.org/pdf/2205.07686.pdf)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2022-ACL, CCF-A) **HIE-SQL**: History Information Enhanced Network for Context-Dependent Text-to-SQL Semantic Parsing
[[paper](https://arxiv.org/pdf/2203.07376v2.pdf)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2022-arXiv, None) Importance of Synthesizing High-quality Data for Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/2212.08785v1.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2021-ACL, CCF-A) Decoupled Dialogue Modeling and Semantic Parsing for Multi-Turn Text-to-SQL
[[paper](https://arxiv.org/pdf/2106.02282v2.pdf)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2021-arXiv, None) Pay More Attention to History: A Context Modelling Strategy for Conversational Text-to-SQL
[[paper](https://arxiv.org/pdf/2112.08735v2.pdf)]
[[code](https://github.com/JuruoMP/RAT-SQL-TC)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)

- (2021-ICLR, CCF-A) **SCORE**: Pre-training for Context Representation in Conversational Semantic Parsing
[[paper](https://openreview.net/pdf?id=oyZxhRI2RiE)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)
[![](https://img.shields.io/badge/MWoZ-blue)](https://github.com/budzianowski/multiwoz)
[![](https://img.shields.io/badge/SQA-red)](https://www.microsoft.com/en-us/download/details.aspx?id=54253)

- (2021-DASFAA, CCF-B) An Interactive NL2SQL Approach with Reuse Strategy
[[paper](https://link.springer.com/chapter/10.1007/978-3-030-73197-7_19)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)

- (2021-NAACL, CCF-B) Structure-Grounded Pretraining for Text-to-SQL
[[paper](https://arxiv.org/pdf/2010.12773v3.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)
[![](https://img.shields.io/badge/WikiSQL-blue)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2021-EMNLP, CCF-B) **PICARD**:Parsing Incrementally for Constrained Auto-Regressive Decoding from Language Models
[[paper](https://arxiv.org/pdf/2109.05093v1.pdf)]
[[code](https://github.com/ServiceNow/picard)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2021-ICLR, CCF-A) **GraPPa**: Grammar-Augmented Pre-Training for Table Semantic Parsing
[[paper](https://arxiv.org/pdf/2009.13845v2.pdf)]
[[code](https://github.com/taoyds/grappa)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/WikiSQL-yellow)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2021-ACL, CCF-A) **LGESQL**: Line Graph Enhanced Text-to-SQL Model with Mixed Local and Non-Local Relations
[[paper](https://arxiv.org/pdf/2106.01093.pdf)]
[[code](https://github.com/rhythmcao/text2sql-lgesql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2020-EMNLP, CCF-B) Bridging Textual and Tabular Data for Cross-Domain Text-to-SQL Semantic Parsing
[[paper](https://arxiv.org/pdf/2012.12627v2.pdf)]
[[code](https://github.com/salesforce/TabularSemanticParsing)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/WikiSQL-yellow)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2020-ACL, CCF-A) **TaBERT**: Pretraining for Joint Understanding of Textual and Tabular Data
[[paper](https://arxiv.org/pdf/2005.08314v1.pdf)]
[[code](https://github.com/facebookresearch/tabert)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/WikiTableQuestions-yellow)](https://github.com/ppasupat/WikiTableQuestions)

- (2020-ACL, CCF-A) **RAT-SQL**: Relation-Aware Schema Encoding and Linking for Text-to-SQL Parsers
[[paper](https://arxiv.org/pdf/1911.04942v5.pdf)]
[[code](https://github.com/Microsoft/rat-sql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/WikiSQL-yellow)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2020-EMNLP, CCF-B) Mention Extraction and Linking for SQL Query Generation
[[paper](https://arxiv.org/pdf/2012.10074v1.pdf)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2020-EMNLP, CCF-B) **IGSQL**: Database Schema Interaction Graph Based Neural Model for Context-Dependent Text-to-SQL Generation
[[paper](https://arxiv.org/pdf/2011.05744v1.pdf)]
[[code](https://github.com/headacheboy/IGSQL)]
[![](https://img.shields.io/badge/SParC-green)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)

- (2020-arXiv, None) Hybrid Ranking Network for Text-to-SQL
[[paper](https://arxiv.org/pdf/2008.04759.pdf)]
[[code](https://github.com/lyuqin/HydraNet-WikiSQL)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2019-arXiv, None) **X-SQL**: reinforce schema representation with context
[[paper](https://arxiv.org/pdf/1908.08113.pdf)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2019-EMNLP, CCF-B) Global Reasoning over Database Structures for Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/1908.11214v1.pdf)]
[[code](https://github.com/benbogin/spider-schema-gnn-global)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2019-EMNLP, CCF-B) Editing-Based SQL Query Generation for Cross-Domain Context-Dependent Questions
[[paper](https://arxiv.org/pdf/1909.00786v2.pdf)]
[[code](https://github.com/ryanzhumich/editsql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/SParC-yellow)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/ATIS-blue)](https://aclanthology.org/H90-1021.pdf)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/SParC-yellow)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/ATIS-blue)](https://aclanthology.org/H90-1021.pdf)

- (2019-ACL, CCF-A) Representing Schema Structure with Graph Neural Networks for Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/1905.06241v2.pdf)]
[[code](https://github.com/benbogin/spider-schema-gnn)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2019-ACL, CCF-A) Towards Complex Text-to-SQL in Cross-Domain Database with Intermediate Representation
[[paper](https://arxiv.org/pdf/1905.08205v2.pdf)]
[[code](https://github.com/microsoft/IRNet)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2018-EMNLP, CCF-B) **SyntaxSQLNet**: Syntax Tree Networks for Complex and Cross-DomainText-to-SQL Task
[[paper](https://arxiv.org/pdf/1810.05237v2.pdf)]
[[code](https://github.com/taoyds/syntaxsql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2018-NAACL, CCF-B) **TypeSQL**: Knowledge-based Type-Aware Neural Text-to-SQL Generation
[[paper](https://arxiv.org/pdf/1804.09769.pdf)]
[[code](https://github.com/taoyds/typesql)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2017-arXiv, None) **SQLNet**: Generating Structured Queries From Natural Language Without Reinforcement Learning
[[paper](https://arxiv.org/pdf/1711.04436.pdf)]
[[code](https://github.com/xiaojunxu/SQLNet)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)



## 🔥 基础模型
- Llama [[paper](https://arxiv.org/pdf/2302.13971.pdf)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023年2月，Meta AI提出开源大模型Llama，有7b、13b、33b、65b共4种规模。

- ChatGLM [[paper](https://arxiv.org/pdf/2103.10360.pdf)] [[code](https://github.com/THUDM/ChatGLM-6B/blob/main/README.md)] [[model](https://huggingface.co/THUDM/chatglm-6b)]
  - 2023年3月，清华大学提出了开源的双语大模型ChatGLM，基于[GLM](https://github.com/THUDM/GLM)框架，参数规格为6b。

- Alpaca [[paper](https://crfm.stanford.edu/2023/03/13/alpaca.html)] [[code](https://github.com/tatsu-lab/stanford_alpaca)] [[model](https://huggingface.co/tatsu-lab/alpaca-7b-wdiff/tree/main)]
  - 2023年3月，斯坦福大学提出基于Llama 7b模型微调的开源大模型Alpaca，有7b共1种规格，训练更简单和便宜。

- Vicuna [[paper](https://lmsys.org/blog/2023-03-30-vicuna/)] [[code](https://github.com/lm-sys/FastChat)] [[model](https://huggingface.co/lmsys)]
  - 2023年3月，UC伯克利大学联合CMU、斯坦福大学提出的开源大模型Vicuna，有7b、13b共2种规格。

- WizardLM [[paper](https://arxiv.org/pdf/2304.12244.pdf)] [[code](https://github.com/nlpxucan/WizardLM)] [[model](https://huggingface.co/WizardLM)]
  - 2023年4月，北京大学和微软提出进化指令大模型WizardLM，有7b、13b、30b共3种规格，2023年6月，提出了数学领域的大模型WizardMath，2023年8月提出了代码领域的大模型WizardCoder。

- Falcon [[paper](https://arxiv.org/pdf/2306.01116.pdf)] [[code](https://huggingface.co/tiiuae/falcon-180B)] [[model](https://huggingface.co/tiiuae)]
  - 2023年6月, 阿联酋提出了大模型Falcon，这是一种仅在网络数据集上训练的开源大模型，具有 1b、7b、40b和180b四个参数规范。值得注意的是，其中Falcon 40B的性能超过了LLaMA 65B。

- ChatGLM2[[paper](https://arxiv.org/pdf/2210.02414.pdf)] [[code](https://github.com/THUDM/ChatGLM2-6B/blob/main/README_EN.md)] [[model](https://huggingface.co/THUDM/chatglm2-6b)]
  - 2023年6月，清华大学提出了ChatGLM的第二代版本ChatGLM 2，规范为6b，具有更强的性能、更长的上下文、更高效的推理和更开放的许可。

- Baichuan-7b [[code](https://github.com/baichuan-inc/baichuan-7B)] [[model](https://huggingface.co/baichuan-inc/Baichuan-7B)]
  - 2023年6月，百川智能提出Baichuan-7B，这是一个基于Transformer架构的开源大规模预训练语言模型，包含70亿个参数，训练了约​​1.2万亿个tokens。支持中文和英文，上下文窗口长度为4096。
  
- Baichuan-13b [[code](https://github.com/baichuan-inc/Baichuan-13B)] [[model](https://huggingface.co/baichuan-inc/Baichuan-13B-Base)]
  - 2023年7月，百川智能继Baichuan-7B之后，提出开源、可商用的大规模语言模型Baichuan-13B，有预训练版本（Baichuan-13B-Base）和对齐版本（Baichuan-13B-Chat）。

- InternLM [[paper](https://github.com/InternLM/InternLM-techreport/blob/main/InternLM.pdf)] [[code](https://github.com/InternLM/InternLM/)] [[model](https://huggingface.co/internlm)]
  - 2023年7月，上海人工智能实验室和商汤科技等提出了InternLM，开源了针对实际场景量身定制的7b和20b参数模型和聊天模型以及训练系统。

- Llama 2 [[paper](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023年7月，Meta AI提出第二代Llama系列开源大模型Llama 2，和Llama 1相比，训练数据多40%，上下文长度翻倍，模型有7b、13b、34b、70b共4种规格，但是34b没有开源。

- Code LLama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023年8月，Meta AI 在 Llama 2 的基础上提出 Code LLama。Code Llama 在多个代码基准测试中达到了开放模型中最先进的性能。有基础模型 (Code Llama)、Python 专业化 (Code Llama - Python) 和指令跟踪模型（instruction-following models），每个模型都有 7B、13B 和 34B 参数。


- Qwen [[paper](https://qianwen-res.oss-cn-beijing.aliyuncs.com/QWEN_TECHNICAL_REPORT.pdf)] [[code](https://github.com/QwenLM/Qwen)] [[model](https://huggingface.co/Qwen)]
  - 2023年8月，阿里云提出大语言模型系列Qwen-7B（简称通义千问），在海量数据上进行预训练，包括网页文本、书籍、代码等，开源了两个版本Qwen-7B和Qwen-7B-Chat。 2023年9月，阿里云更新了Qwen-7B和Qwen-7B-Chat，并开源了Qwen-14B和Qwen-14B-Chat。

- Baichuan 2 [[code](https://github.com/baichuan-inc/Baichuan2)] [[model](https://huggingface.co/baichuan-inc)]
  - 2023年9月，百川智能提出新一代开源大语言模型Baichuan 2，在2.6万亿个tokens的高质量语料上训练，有7B和13B的基础版和聊天版，以及4bits量化版聊天模型。

- Phi-1.5 [[paper](https://arxiv.org/pdf/2309.05463.pdf)] [[model](https://huggingface.co/microsoft/phi-1_5)]
  - 2023年9月，微软研究院提出开源语言模型phi-1.5，一个拥有1.3b个参数的Transformer，使用与[phi-1](https://huggingface.co/microsoft/phi-1)相同的数据源进行训练，增加了由各种NLP合成文本组成的新数据源。当根据测试常识、语言理解和逻辑推理的基准进行评估时，phi-1.5在参数少于10b的模型中表现出近乎最先进的性能。

 ## 💡 微调
- P-Tuning [[paper](https://arxiv.org/pdf/2103.10385.pdf)] [[code](https://github.com/THUDM/P-tuning)] 
  - 2021年3月，清华大学等提出了针对大模型微调方法P-Tuning，采用可训练的连续提示词嵌入，降低了微调成本。

- LoRA [[paper](https://arxiv.org/pdf/2106.09685.pdf)] [[code](https://github.com/microsoft/LoRA)] 
  - 2021年6月，微软提出的针对大模型微调的Low-Rank Adaptation（LoRA）方法，冻结预训练权重。

- P-Tuning V2 [[paper](https://arxiv.org/pdf/2110.07602.pdf)] [[code](https://github.com/THUDM/P-tuning-v2)] 
  - 2021年10月，清华大学提出了P-Tuning的改进版本P-Tuning V2，性能更优。

- RLHF [[paper](https://huggingface.co/blog/rlhf)] [[code](https://github.com/huggingface/blog/blob/main/zh/rlhf.md)] 
  - 2022年12月，OpenAI使用RLHF方法训练ChatGPT，利用人类反馈信号直接优化语言模型，表现优异。

- RRHF [[paper](https://arxiv.org/pdf/2304.05302.pdf)] [[code](https://github.com/GanjinZero/RRHF)] 
  - 2023年4月，阿里巴巴提出了一种新的学习范式称为RRHF（Rank Responses to Align Language Models with Human Feedback without tears），可以像微调一样轻松调整并实现PPO算法在HH数据集中的性能。

- QLoRA [[paper](https://arxiv.org/pdf/2305.14314.pdf)] [[code](https://github.com/artidoro/qlora)] 
  - 2023年5月，华盛顿大学基于冻结的4bit量化模型，结合LoRA方法训练，进一步降低了微调门槛。

- RLTF [[paper](https://arxiv.org/pdf/2307.04349.pdf)] [[code](https://github.com/Zyq-scut/RLTF)] 
  - 2023年7月，腾讯提出了RLTF（Reinforcement Learning from Unit Test Feedback），这是一种新颖的online强化学习框架，具有多粒度的单元测试反馈，用于细化code LLMs。

- RRTF [[paper](https://arxiv.org/pdf/2307.14936v1.pdf)]
  - 2023年7月，华为提出RRTF（Rank Responses toalign Test&Teacher Feedback）。与 RLHF 相比，RRHF可以有效地将语言模型的输出概率与人类偏好对齐，调优期间只需要1-2个模型，并且在实现、超参数调优和训练方面比PPO更简单。

- RLAIF [[paper](https://arxiv.org/pdf/2309.00267.pdf)]
  - 2023年9月，谷歌提出了RLAIF（来自AI反馈的强化学习RL），这是一种由现成的LLM代替人类来标记偏好的技术。他们发现RLHF和 RLAIF方法在摘要任务上取得了相似的结果。

## 💪 数据集
- WikiSQL [[paper](https://arxiv.org/pdf/1709.00103.pdf)] [[code](https://github.com/salesforce/WikiSQL)] [[dataset](https://github.com/salesforce/WikiSQL)]
  - 2017年9月，Salesforce提出的一个大型的Text-to-SQL数据集，数据来源于Wikipedia，属于单领域，包含了80654个自然语言问题，77840个SQL语句，SQL语句形式比较简单，不包含排序、分组、子查询等复杂操作。

- Spider [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider)] [[dataset](https://yale-lily.github.io/spider)]
  - 2018年9月，耶鲁大学提出的多数据库、多表、单轮查询的Text-to-SQL数据集，也是业界公认难度最大的大规模跨领域评测榜单，包含了10181个自然语言问题，5693个SQL语句，涉及138个不同领域的200多个数据库，难易程度分为：简单、中等、困难、特别困难。

- SParC [[paper](https://arxiv.org/pdf/1906.02285.pdf)] [[code](https://github.com/taoyds/sparc)] [[dataset](https://drive.google.com/uc?export=download&id=1Uu7NMHTR1tdQw1t7bAuM7OPU4LElVKfg)]
  - 2019年6月，耶鲁大学提出了一个大型数据集SParC，用于复杂、跨域、上下文相关（多轮）语义解析和Text-to-SQL任务，该数据集由4298个连贯的问题序列组成（有12k+个自然语言问题到SQL标注的Question-SQL对，由14名耶鲁大学学生标注），通过用户与138个领域的200个复杂数据库的交互获得。

- CSpider [[paper](https://arxiv.org/pdf/1909.13293.pdf)] [[code](https://github.com/taolusi/chisp)] [[dataset](https://drive.google.com/drive/folders/1TxCUq1ydPuBdDdHF3MkHT-8zixluQuLa?usp=sharing)]
  - 2019年9月，西湖大学提出了一个大型中文数据集CSpider，用于复杂和跨领域的语义解析和Text-to-SQL任务，由2位NLP研究人员和1位计算机专业学生从数据集Spider翻译而来，其中包含200个数据库上的10181个问题和5693个独特的复杂SQL查询，具有涵盖138个不同领域的多个表的数据库。

- CoSQL [[paper](https://arxiv.org/pdf/1909.05378.pdf)] [[code](https://yale-lily.github.io/cosql)] [[dataset](https://yale-lily.github.io/cosql)]
  - 2019年9月，耶鲁大学和Salesforce Research提出了一种跨域数据库CoSQL，它由30k+轮次和10k+带注释的SQL查询组成，这些查询是从Wizard-of-Oz (WOZ)集合中获得的，该集合包含3k个对话，查询跨越 138个域的200个复杂数据库。

- TableQA [[paper](https://arxiv.org/pdf/2006.06434.pdf)] [[dataset](https://www.luge.ai/#/luge/dataDetail?id=12)]
  - 2020年6月，追一科技公司提出了一个大规模跨领域Text-to-SQL数据集TableQA，其中包含64891个问题和6000多个表的20311个唯一SQL查询。

- DuSQL [[paper](https://aclanthology.org/2020.emnlp-main.562.pdf)] [[dataset](https://www.luge.ai/#/luge/dataDetail?id=13)]
  - 2020年11月，百度针对跨域文本到SQL任务提出了一个大规模、实用的中文数据集DuSQL，它包含200个数据库、813个表和23797个Question-SQL对。

- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase)] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
  - 2021年8月，西安交通大学和微软等提出了首个跨领域、多轮Text-to-SQL中文数据集，包含了5459个多轮问题组成的列表，17940个<query, SQL>二元组。

- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)] [[dataset](https://bird-bench.github.io/)]
  - 2023年5月，香港大学和阿里巴巴提出了一个大规模跨域数据集BIRD，其中包含超过12751个独特的问题 SQL、95个大数据库，总大小为33.4GB。它还涵盖区块链、曲棍球、医疗保健和教育等超过37个专业领域。

## 🌈 评测指标
- Execution Accuracy (EX) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - 定义：计算SQL执行结果正确的数量在数据集中的比例，结果存在高估的可能。

- Exact Match (EM) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - 定义：计算模型生成的SQL和标注SQL的匹配程度，结果存在低估的可能。


## 🔧 实践项目
- [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) 
[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/DB-GPT-Hub?style=social)](https://github.com/eosphoros-ai/DB-GPT-Hub/stargazers)
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/DB-GPT-Hub?color=green)
  - eosphoros组织提出的专注于大模型Text-to-SQL微调的开源项目，包含了大模型下载、数据集预处理、LoRA和QLoRA等微调技术、模型预测、模型评估等步骤。

- [sqlcoder](https://github.com/defog-ai/sqlcoder)
[![GitHub Repo stars](https://img.shields.io/github/stars/defog-ai/sqlcoder?style=social)](https://github.com/defog-ai/sqlcoder/stargazers)
![last commit](https://img.shields.io/github/last-commit/defog-ai/sqlcoder?color=green)
  - Defog组织提出的先进的Text-to-SQL的大模型，表现亮眼，效果优于GPT3.5、wizardcoder和starcoder等，仅次于GPT4。

- [modal_finetune_sql](https://github.com/run-llama/modal_finetune_sql)
[![GitHub Repo stars](https://img.shields.io/github/stars/run-llama/modal_finetune_sql?style=social)](https://github.com/run-llama/modal_finetune_sql/stargazers)
![last commit](https://img.shields.io/github/last-commit/run-llama/modal_finetune_sql?color=green)
  - 项目基于LLaMa 2 7b模型进行Text-to-SQL微调，有完整的训练、微调、评估流程。

- [LLaMA-Efficient-Tuning](https://github.com/hiyouga/LLaMA-Efficient-Tuning) 
[![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/stargazers)
![last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning?color=green)
  - 这是一个易于使用的LLM微调框架，支持LLaMA-2、BLOOM、Falcon、Baichuan、Qwen、ChatGLM2等。


## 🤝 友情链接
- [eosphoros](https://github.com/eosphoros-ai)
[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai?style=social)](https://github.com/eosphoros-ai)
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/DB-GPT?color=green)
  - 他们是一支由来自互联网公司的技术爱好者和热衷于开源项目的NLP研究生组成的团队。他们的重点是开发保护数据库和大型语言模型的隐私和安全的解决方案。他们的目标是确保这些模型的能力保持绝对私密、安全和受控。

- [Awesome-AIGC-Tutorials](https://github.com/luban-agi/Awesome-AIGC-Tutorials)
[![GitHub Repo stars](https://img.shields.io/github/stars/luban-agi/Awesome-AIGC-Tutorials?style=social)](https://github.com/luban-agi/Awesome-AIGC-Tutorials/stargazers)
![last commit](https://img.shields.io/github/last-commit/luban-agi/Awesome-AIGC-Tutorials?color=green)
  - Awesome AIGC Tutorials 包含一系列精选的教程和资源，涵盖大型语言模型、AI 绘画和相关领域。探索适合初学者和高级人工智能爱好者的深入见解和知识。

[![Star History Chart](https://api.star-history.com/svg?repos=eosphoros-ai/Awesome-Text2SQL&type=Date)](https://star-history.com/#eosphoros-ai/Awesome-Text2SQL)
