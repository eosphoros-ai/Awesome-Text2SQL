# **Awesome Text2SQL**🎉🎉🎉


[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://img.shields.io/badge/Awesome-green.svg)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![Last Commit](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)


[**English**](README.md) | **中文版** | [**论文**](https://arxiv.org/abs/2406.11434)

这里收集了针对大型语言模型、Text2SQL、[Text2DSL](Text2DSL.md)、 [Text2API](Text2API.md)、 [Text2Vis](Text2Vis.md) 等的精选教程和资源。

## 🌱 如何贡献
我们热烈欢迎大家的贡献，无论您是发现拼写错误、错误、有建议，还是想要分享与LLM+Text2SQL相关的资源。有关如何贡献的详细指南，请参阅我们的 [CONTRIBUTING.md](CONTRIBUTING.md) 文件。

## 🔔 排行榜


|       |                              [WikiSQL](https://github.com/salesforce/WikiSQL#leaderboard)                               |                [Spider](https://yale-lily.github.io/spider)<br/>Exact Match(EM)                 |              [Spider](https://yale-lily.github.io/spider)<br/>Exact Execution(EX)               | [BIRD](https://bird-bench.github.io/)<br/> Reward-based Valid Efficiency Score (R-VES) |        [BIRD](https://bird-bench.github.io/)<br/>Execution Accuracy (EX)        |
| :---: | :---------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: |:--------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
|  🏆1   |             **93.0** <br/>(2021/05-[SeaD+Execution-Guided Decoding](https://arxiv.org/pdf/2105.07911.pdf))              |                                **81.5** <br/>(2023/11-MiniSeek)                                 |                                **91.2** <br/>(2023/11-MiniSeek)                                 |                  **69.36** <br/>(2024/08-OpenSearch-SQL, v2 + GPT-4o)                  | **73.00** <br/>(2024/09-[CHASE-SQL + Gemini](https://arxiv.org/abs/2410.01943)) |
|  🥈2   |               92.7 <br/>(2021/03-[SDSQL+Execution-Guided Decoding](https://arxiv.org/pdf/2103.04399.pdf))               |         74.0 <br/>(2022/09-[Graphix-3B + PICARD](https://arxiv.org/pdf/2301.07507.pdf))         | 86.6 <br/>(2023/08-[DAIL-SQL + GPT-4 + Self-Consistency](https://arxiv.org/pdf/2308.15363.pdf)) |                      68.79 <br/>(2024/08-ExSL + granite-34b-code)                      |                      72.39 <br/>(2024/09-AskData + GPT-4o)                      |
|  🥉3   |        92.5 <br/>(2020/11-[IE-SQL+Execution-Guided Decoding](https://aclanthology.org/2020.emnlp-main.563.pdf))         |                               73.9 <br/>(2022/09-CatSQL + GraPPa)                               |          86.2 <br/>(2023/08-[DAIL-SQL + GPT-4](https://arxiv.org/pdf/2308.15363.pdf))           |      68.44 <br/>(2024/09-[CHASE-SQL + Gemini](https://arxiv.org/abs/2410.01943))       |                72.28 <br/>(2024/08-OpenSearch-SQL, v2 + GPT-4o)                 |
|   4   |             92.2 <br/>(2020/03-[HydraNet+Execution-Guided Decoding](https://arxiv.org/pdf/2008.04759.pdf))              |            73.1 <br/>(2022/09-[SHiP + PICARD](https://arxiv.org/pdf/2212.08785.pdf))            |                      85.6 <br/>(2023/10-DPG-SQL + GPT-4 + Self-Correction)                      |      67.41 <br/>(2024/07-[Distillery + GPT-4o](https://arxiv.org/abs/2408.07702))      |  71.83 <br/>(2024/07-[Distillery + GPT-4o](https://arxiv.org/abs/2408.07702))   |
|   5   |              91.9 <br/>(2020/12-[BRIDGE+Execution-Guided Decoding](https://arxiv.org/pdf/2012.12627.pdf))               | 72.9 <br/>(2022/05-[G³R + LGESQL + ELECTRA](https://aclanthology.org/2023.findings-acl.23.pdf)) |           85.3 <br/>(2023/04-[DIN-SQL + GPT-4](https://arxiv.org/pdf/2304.11015.pdf))           |                         66.92 <br/>(2024/09-AskData + GPT-4o)                          |                  70.37 <br/>(2024/08-ExSL + granite-34b-code)                   |
|   6   |               91.8 <br/>(2019/08-[X-SQL+Execution-Guided Decoding](https://arxiv.org/pdf/1908.08113.pdf))               |                          72.4 <br/>(2022/08-RESDSQL+T5-1.1-lm100k-xl)                           |                    83.9 <br/>(2023/07-Hindsight Chain of Thought with GPT-4)                    |                            66.39 <br/>(2024/08-Insights AI)                            |                        70.26 <br/>(2024/08-Insights AI)                         |
|   7   |                            91.4 <br/>(2021/03-[SDSQL](https://arxiv.org/pdf/2103.04399.pdf))                            |                                    72.4 <br/>(2022/05-T5-SR)                                    |      82.3 <br/>(2023/06-[C3 + ChatGPT + Zero-Shot](https://arxiv.org/pdf/2307.07306.pdf))       |                      66.25 <br/>(2024/05-ExSL + granite-20b-code)                      |                   70.21 <br/>(2024/07-PURPLE + RED + GPT-4o）                    |
|   8   |                           91.1 <br/>(2020/12-[BRIDGE](https://arxiv.org/pdf/2012.12627.pdf))                            |   72.2 <br/>(2022/12-[N-best List Rerankers + PICARD](https://arxiv.org/pdf/2210.10668.pdf))    |           80.8 <br/>(2023/07-Hindsight Chain of Thought with GPT-4 and Instructions)            |                          65.70 <br/>(2024/07-RECAP + Gemini)                           |                       69.03 <br/>(2024/07-RECAP + Gemini)                       |
|   9   | 91.0 <br/>(2021/04-[Text2SQLGen + EG](https://www.semanticscholar.org/reader/b877233410484b2ff2add278105c53b6633d9d20)) |          72.1 <br/>(2021/09-[S²SQL + ELECTRA ](https://arxiv.org/pdf/2203.06958.pdf))           |         79.9 <br/>(2023/02-[RESDSQL-3B + NatSQ](https://arxiv.org/pdf/2302.05965.pdf))          |                       65.62 <br/>(2024/07-PURPLE + RED + GPT-4o）                       |                         68.87 <br/>(2024/07-ByteBrain)                          |
|  10   |                        90.5 <br/>(2020/11-[SeqGenSQL+EG](https://arxiv.org/pdf/2011.03836.pdf))                         |         72.0 <br/>(2023/02-[RESDSQL-3B + NatSQL](https://arxiv.org/pdf/2302.05965.pdf))         |                                 78.5 <br/>(2022/11-SeaD + PQL)                                  |                         63.68 <br/>(2024/08-Arcwise + GPT-4o）                          |                  67.86 <br/>(2024/05-ExSL + granite-20b-code)                   |


## 📜 目录
- [**Awesome Text2SQL**🎉🎉🎉](#awesome-text2sql)
  - [🌱 如何贡献](#-如何贡献)
  - [🔔 排行榜](#-排行榜)
  - [📜 目录](#-目录)
  - [👋 简介](#-简介)
  - [📖 综述](#-综述)
  - [💬 经典模型](#-经典模型)
  - [🔥 基础模型](#-基础模型)
  - [💡 微调](#-微调)
  - [💪 数据集](#-数据集)
  - [🌈 评测指标](#-评测指标)
  - [📦 库函数](#-库函数)
  - [🔧 实践项目](#-实践项目)
  - [🔗 引用](#-引用)
  - [🤝 友情链接](#-友情链接)


## 👋 简介
- Text-to-SQL（或者Text2SQL），顾名思义就是把文本转化为SQL语言，更学术一点的定义是：把数据库领域下的自然语言（Natural Language，NL）问题，转化为在关系型数据库中可以执行的结构化询语言（Structured Query Language，SQL），因此Text-to-SQL也可以被简写为NL2SQL。
  - 输入：自然语言问题，比如“*查询表t_user的相关信息，结果按id降序排序，只保留前10个数据*”
  - 输出：SQL，比如“*SELECT * FROM t_user ORDER BY id DESC LIMIT 10*”


## 📖 综述
- (2025-TKDE, CCF-A) Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL
[[paper](https://arxiv.org/pdf/2406.08426)]
[[code](https://github.com/DEEP-PolyU/Awesome-LLM-based-Text2SQL)]

- (2024-arXiv) From Natural Language to SQL: Review of LLM-based Text-to-SQL Systems
[[paper](https://arxiv.org/pdf/2410.01066)]

- (2024-arXiv) Large Language Model Enhanced Text-to-SQL Generation: A Survey
[[paper](https://arxiv.org/pdf/2410.06011)]

- (2024-arXiv) A Survey of NL2SQL with Large Language Models: Where are we, and where are we going? 
[[paper](https://arxiv.org/pdf/2408.05109)]
[[code](https://github.com/HKUSTDial/NL2SQL_Handbook)]

- (2024-arXiv) A Survey on Employing Large Language Models for Text-to-SQL Tasks 
[[paper](https://arxiv.org/pdf/2407.15186)]

- (2023-VLDB, CCF-A）A survey on deep learning approaches for text-to-SQL 
[[paper](https://link.springer.com/article/10.1007/s00778-022-00776-8)]

- (2022-TKDE, CCF-A) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions 
[[paper](https://arxiv.org/pdf/2208.13629.pdf)]

- (2022-COLOING, CCF-B) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect 
[[paper](https://arxiv.org/pdf/2208.10099v1.pdf)]

- (2022-arXiv)Deep Learning Driven Natural Languages Text to SQL Query Conversion: A Survey 
[[paper](https://arxiv.org/pdf/2208.04415.pdf)]

## 💬 经典模型
- (2025-NAACL, CCF-B) **You Only Read Once (YORO)**: Learning to Internalize Database Knowledge for Text-to-SQL
[[paper](https://aclanthology.org/2025.naacl-long.94/)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)
[![](https://img.shields.io/badge/KaggleDBQA-red)](https://github.com/Chia-Hsuan-Lee/KaggleDBQA)

- (2025-EDBT, CCF-B) **DBCᴏᴘɪʟᴏᴛ**: Natural Language Querying over Massive Databases via Schema Routing
 [[paper](https://arxiv.org/pdf/2312.03463.pdf)]
 [[code](https://github.com/tshu-w/DBCopilot)]
 [![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
 [![](https://img.shields.io/badge/Spider--Realistic-yellow)](https://aclanthology.org/2021.naacl-main.105.pdf)
 [![](https://img.shields.io/badge/Spider--Syn-blue)](https://arxiv.org/pdf/2106.01065.pdf)
 [![](https://img.shields.io/badge/BIRD-red)](https://bird-bench.github.io/)

- (2024-arXiv, None) **CHASE-SQL**: Multi-Path Reasoning and Preference Optimized Candidate Selection in Text-to-SQL
[[paper](https://arxiv.org/abs/2410.01943)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2024-arXiv, None) **E-SQL**: Direct Schema Linking via Question Enrichment in Text-to-SQL
[[paper](https://arxiv.org/abs/2409.16751)]
[[code](https://github.com/HasanAlpCaferoglu/E-SQL)]
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2024-arXiv, None) **Distillery**: The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models
[[paper](https://arxiv.org/abs/2408.07702)]
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2024-arXiv, None) **DB-GPT-Hub**: Towards Open Benchmarking Text-to-SQL Empowered by Large Language Models
[[paper](https://arxiv.org/pdf/2406.11434)]
[[code](https://github.com/eosphoros-ai/DB-GPT-Hub)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2024-arXiv, None) **SuperSQL**: The Dawn of Natural Language to SQL: Are We Fully Ready?
[[paper](https://arxiv.org/abs/2406.01265)]
[[code](https://github.com/HKUSTDial/NL2SQL360)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2024-arXiv, None) **CHESS**: Contextual Harnessing for Efficient SQL Synthesis
[[paper](https://arxiv.org/abs/2405.16755)]
[[code](https://github.com/ShayanTalaei/CHESS)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

- (2023-arXiv, None) **MAC-SQL**: A Multi-Agent Collaborative Framework for Text-to-SQL
[[paper](https://arxiv.org/pdf/2312.11242.pdf)]
[[code](https://github.com/wbbeyourself/MAC-SQL)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

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

- (2019-arXiv, None) **X-SQL**: reinforce schema representation with context
[[paper](https://arxiv.org/pdf/1908.08113.pdf)]
[![](https://img.shields.io/badge/WikiSQL-green)](https://github.com/salesforce/WikiSQL/blob/master/README.md)

- (2019-EMNLP, CCF-B) Global Reasoning over Database Structures for Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/1908.11214v1.pdf)]
[[code](https://github.com/benbogin/spider-schema-gnn-global)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2019-EMNLP, CCF-B) Editing-Based SQL Query Generation for Cross-Domain Context-Dependent Questions
[[paper](https://arxiv.org/pdf/1909.00786v2.pdf)]
[[code](https://github.com/ryanzhumich/editsql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/SParC-yellow)](https://arxiv.org/pdf/1906.02285.pdf)
[![](https://img.shields.io/badge/ATIS-blue)](https://aclanthology.org/H90-1021.pdf)

- (2019-ACL, CCF-A) Representing Schema Structure with Graph Neural Networks for Text-to-SQL Parsing
[[paper](https://arxiv.org/pdf/1905.06241v2.pdf)]
[[code](https://github.com/benbogin/spider-schema-gnn)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2019-ACL, CCF-A) Towards Complex Text-to-SQL in Cross-Domain Database with Intermediate Representation
[[paper](https://arxiv.org/pdf/1905.08205v2.pdf)]
[[code](https://github.com/microsoft/IRNet)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2018-EMNLP, CCF-B) **SyntaxSQLNet**: Syntax Tree Networks for Complex and Cross-DomainText-to-SQL Task
[[paper](https://arxiv.org/pdf/1810.05237v2.pdf)]
[[code](https://github.com/taoyds/syntaxsql)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)

- (2018-NAACL, CCF-B) **TypeSQL**: Knowledge-based Type-Aware Neural Text-to-SQL Generation
[[paper](https://arxiv.org/pdf/1804.09769.pdf)]
[[code](https://github.com/taoyds/typesql)]
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

- Code Llama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023年8月，Meta AI 在 Llama 2 的基础上提出 Code LLama。Code Llama 在多个代码基准测试中达到了开放模型中最先进的性能。有基础模型 (Code Llama)、Python 专业化 (Code Llama - Python) 和指令跟踪模型（instruction-following models），每个模型都有 7B、13B 和 34B 参数。2024年1月，Meta AI开源CodeLLama-70b、CodeLLama-70b-Python和CodeLLama-70b-Instruct。


- Qwen [[paper](https://qianwen-res.oss-cn-beijing.aliyuncs.com/QWEN_TECHNICAL_REPORT.pdf)] [[code](https://github.com/QwenLM/Qwen)] [[model](https://huggingface.co/Qwen)]
  - 2023年8月，阿里云提出大语言模型系列Qwen-7B（简称通义千问），在海量数据上进行预训练，包括网页文本、书籍、代码等，开源了两个版本Qwen-7B和Qwen-7B-Chat。 2023年9月，阿里云更新了Qwen-7B和Qwen-7B-Chat，并开源了Qwen-14B和Qwen-14B-Chat。2023年11月, 他们开源了Qwen-1.8B，Qwen-1.8B-Chat，Qwen-72B以及Qwen-72B-Chat.

- Baichuan 2  [[paper](https://arxiv.org/pdf/2309.10305.pdf)]
[[code](https://github.com/baichuan-inc/Baichuan2)] [[model](https://huggingface.co/baichuan-inc)]
  - 2023年9月，百川智能提出新一代开源大语言模型Baichuan 2，在2.6万亿个tokens的高质量语料上训练，有7B和13B的基础版和聊天版，以及4bits量化版聊天模型。

- Phi-1.5 [[paper](https://arxiv.org/pdf/2309.05463.pdf)] [[model](https://huggingface.co/microsoft/phi-1_5)]
  - 2023年9月，微软研究院提出开源语言模型phi-1.5，一个拥有1.3b个参数的Transformer，使用与[phi-1](https://huggingface.co/microsoft/phi-1)相同的数据源进行训练，增加了由各种NLP合成文本组成的新数据源。当根据测试常识、语言理解和逻辑推理的基准进行评估时，phi-1.5在参数少于10b的模型中表现出近乎最先进的性能。2023年12月，他们提出了[Phi-2](https://huggingface.co/microsoft/phi-2)，一个 2.7b参数的语言模型，展示了出色的推理和语言理解能力，展示了参数少于13b的基础语言模型中最先进的性能。

 - Mistral-7B [[paper](https://arxiv.org/pdf/2310.06825.pdf)] 
   [[code](https://github.com/mistralai/mistral-src)] 
   [[model](https://huggingface.co/mistralai/Mistral-7B-v0.1)]
   - 2023年10月，Mistral-AI 公司提出开源 LLM Mistral 7B，这是一个具有7b参数的语言模型，旨在实现卓越的性能和效率。Mistral 7B 在所有评估基准中均优于开源的llama2 13B，在推理、数学和代码生成方面优于llama1-34B模型。他们还提供了一个经过微调以遵循指令的模型Mistral 7B–Instruct，该模型在人类和自动化基准测试上都超越了Llama2-13B-Chat。2023年12月，他们提出了开源LLM Mixtral-8x7B，一种预训练的生成式稀疏专家混合物，在大多数基准测试上优于Llama2 70B。 

 - Deepseek [[paper](https://arxiv.org/pdf/2401.02954.pdf)] 
   [[code](https://github.com/deepseek-ai/DeepSeek-LLM)] 
   [[model](https://huggingface.co/deepseek-ai)]
   - 2023年11月, DeepSeek-AI公司提出了开源LLM deepseek，它是在包含2万亿个中英文token的庞大数据集上从头开始训练的。同样，deepseek LLM主要有base和chat两大类，分别有7b和67b两种参数格式。论文中的数据显示，deepSeek LLM 67b 在一系列基准测试中都超越了LLaMA2 70b，特别是在代码、数学和推理领域。 此外，与GPT-3.5相比，DeepSeek LLM 67B Chat 表现出卓越的性能。

 - MiniCPM [[paper](https://shengdinghu.notion.site/MiniCPM-c805a17c5c8046398914e47f0542095a)]
    [[code](https://github.com/OpenBMB/MiniCPM)] 
    [[model](https://huggingface.co/openbmb)]
   - 2024年2月, 面壁智能与清华大学自然语言处理实验室开源了大模型MiniCPM，这是一个系列端侧大模型，主体语言模型 MiniCPM-2B 仅有 24亿（2.4B）的非词嵌入参数量, 总计2.7B参数量。值得注意的是，经过 SFT 后，MiniCPM 在公开综合性评测集上，MiniCPM 与 Mistral-7B相近（中文、数学、代码能力更优），整体性能超越 Llama2-13B、MPT-30B、Falcon-40B 等模型。

 - Mixtral-8x22B [[paper](https://mistral.ai/news/mixtral-8x22b/)][[code](https://docs.mistral.ai/getting-started/open_weight_models/)] [[model](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1)]
   - 2024年4月, Mistral AI提出了最新的开源模型 Mixtral 8x22B。 它为人工智能社区的性能和效率设立了新标准。 它是一个稀疏专家混合 (SMoE) 模型，仅使用 141B 个活动参数中的 39B 个，在其规模下提供了无与伦比的成本效率。


 - Phi-3 [[paper](https://azure.microsoft.com/en-us/blog/introducing-phi-3-redefining-whats-possible-with-slms/)] [[model](https://huggingface.co/microsoft/Phi-3-mini-128k-instruct)]
   - 2024年4月, 微软提出了 Phi-3 模型，这是现有的功能最强大、最具成本效益的小语言模型 (SLM)，在各种语言、推理、编码和计算方面，其性能优于相同大小和更高大小的模型。 数学基准。 Phi-3-mini 有两种上下文长度变体 4K 和 128K 令牌。 它是同类产品中第一个支持最多 128K 个令牌的上下文窗口的模型，对质量影响很小。 Phi-3-small (7B) 和 Phi-3-medium (14B) 很快就会在 Azure AI 模型目录和其他模型花园中提供。


  - Llama 3 [[paper](https://ai.meta.com/blog/meta-llama-3/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
    - 2024年4月，Meta AI提出第三代Llama系列开源大模型Llama 3，模型有8b、70b共2种参数规格, 每种规则都有base和instruct版本。令人兴奋的是，Llama 3 模型是 Llama 2 的重大飞跃，并为这些参数规模的 LLM 模型建立了新的最先进水平。

  - Qwen-1.5-110B [[paper](https://qwenlm.github.io/blog/qwen1.5-110b/)] [[code](https://github.com/QwenLM/Qwen1.5)] [[model](https://huggingface.co/Qwen/Qwen1.5-110B)]
    - 2024年4月, 阿里云提出Qwen1.5系列首个100B+模型Qwen1.5-110B，该模型在基础模型评测中达到与Meta-Llama3-70B相当的性能，在包括MT-Bench和AlpacaEval 2.0在内的聊天评测中表现出色。Qwen1.5是Qwen2的测试版，有9种模型尺寸，包括0.5B、1.8B、4B、7B、14B、32B、72B和110B密集模型，以及14B激活2.7B的MoE模型。
  
  - Qwen2 [[paper](https://qwenlm.github.io/blog/qwen2/)] [[code](https://github.com/QwenLM/Qwen2)] [[model](https://huggingface.co/collections/Qwen/qwen2-6659360b33528ced941e557f)]
    - 2024年6月，阿里云提出从Qwen1.5演进到Qwen2，Qwen2有5个模型尺寸，包括Qwen2-0.5B、Qwen2-1.5B、Qwen2-7B、Qwen2-57B-A14B、Qwen2-72B。Qwen2-72B相比Llama-3-70B等领先模型表现出色，尤其在参数更少的情况下，超越了上一代Qwen1.5-110B的性能。

   - Llama 3.1  [[paper](https://ai.meta.com/blog/meta-llama-3-1/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
     - 2024年7月, Meta AI 推出了 Llama 3.1 405B，这是第一个公开可用的模型，在常识、可操纵性、数学、工具使用和多语言翻译等最先进的能力方面可与顶级 AI 模型相媲美。作为最新版本的一部分，他们推出了 8B 和 70B 模型的升级版。它们是多语言的，具有明显更长的 128K 上下文长度、最先进的工具使用和整体更强大的推理能力。

  - Qwen2.5 [[paper](https://arxiv.org/abs/2407.10671)] [[code](https://github.com/QwenLM/Qwen2.5)] [[model](https://huggingface.co/Qwen)]
    - 2024年9月, 2024/09，阿里云发布了Qwen家族的最新成员：Qwen2.5，以及专门用于编码的Qwen2.5-Coder和数学的Qwen2.5-Math。所有开放权重模型都是密集的、仅用于解码器的语言模型，有多种大小可供选择，包括：Qwen2.5（0.5B、1.5B、3B、7B、14B、32B和72B），Qwen2.5-Coder（1.5B、7B和32B正在开发中）和Qwen2.5-Math（1.5B、7B和72B）。他们将其最大的开源模型Qwen2.5-72B-Instruct与领先的开源模型Llama-3.1-70B-Instrct和Mistral-Large-V2-Instruct进行了对标，在多个指标上取得了最佳成绩。除了指令调整的语言模型之外，他们还发现 Qwen2.5-72B 即使与像 Llama-3-405B 这样的更大的模型相比也能达到顶级性能。
    
   - Llama 3.2  [[paper](https://ai.meta.com/blog/llama-3-2-connect-2024-vision-edge-mobile-devices/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
     - 2024年9月, Meta AI 提出了 Llama 3.2，其中包括小型和中型视觉 LLM（11B 和 90B）以及适合边缘和移动设备的轻量级纯文本模型（1B 和 3B），包括预训练和指令调整版本。Llama 3.2 1B 和 3B 模型支持 128K 令牌的上下文长度，并且是同类产品中最先进的，适用于总结、指令跟踪和在边缘本地运行的重写任务等设备用例。这些模型在第一天就适用于 Qualcomm 和联发科硬件，并针对 Arm 处理器进行了优化。

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
  - 2018年9月，耶鲁大学提出的多数据库、多表、单轮查询的Text-to-SQL数据集，也是业界公认难度最大的大规模跨领域评测榜单，包含了10181个自然语言问题，5693个SQL语句，涉及138个不同领域的200多个数据库，难易程度分为：简单、中等、困难、特别困难。2024年2月，耶鲁大学开源了Spider1.0排行榜单的test数据集，并且他们将在3月开源Spider 2.0数据集。

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

- KaggleDBQA [[paper](https://arxiv.org/abs/2106.11455)] [[code](https://github.com/Chia-Hsuan-Lee/KaggleDBQA/)] [[dataset](https://github.com/Chia-Hsuan-Lee/KaggleDBQA/tree/main?tab=readme-ov-file#Data-Format)]
  - 2021年6月，华盛顿大学和微软研究院提出了KaggleDBQA，这是一个真实Web数据库的跨域评估数据集，具有特定领域的数据类型、原始格式和不受限制的问题。 它包括跨 8 个数据库的 272 个示例，每个数据库平均有 2.25 个表。 该数据集以其真实世界的数据源、自然的问题创作环境以及具有丰富领域知识的数据库文档而闻名。 主要统计数据：8.7% WHERE 子句、73.5% VAL、24.6% SELECT 和 6.8% NON-SELECT。

- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase)] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
  - 2021年8月，西安交通大学和微软等提出了首个跨领域、多轮Text-to-SQL中文数据集，包含了5459个多轮问题组成的列表，17940个<query, SQL>二元组。

- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)] [[dataset](https://bird-bench.github.io/)]
  - 2023年5月，香港大学和阿里巴巴提出了一个大规模跨域数据集BIRD，其中包含超过12751个独特的问题 SQL、95个大数据库，总大小为33.4GB。它还涵盖区块链、曲棍球、医疗保健和教育等超过37个专业领域。

- BIRD-SQL Mini-Dev [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/bird-bench/mini_dev)] [[dataset](https://bird-bench.github.io/)]
  - 2024年6月，香港大学与阿里巴巴继续合作，发布 BIRD-SQL Mini-Dev，这是其开发数据集的精简版，旨在高效且经济高效地测试SQL模型。该数据集从11个不同的数据库中编译了500个高质量的text2SQL对，并支持MySQL和PostgreSQL格式。它引入了两个新的评估指标：基于奖励的有效效率分数 (R-VES) 和F1-Score，这两个指标目前都处于测试阶段，专门为在开发环境中提高文本到SQL模型的准确性和效率而开发。

- Spider 2.0 [[paper](https://spider2-sql.github.io/)] [[code](https://github.com/xlang-ai/Spider2)] [[dataset](https://github.com/xlang-ai/Spider2)]
  - 2024年8月, XLang AI 提出的 Spider 2.0数据集是针对实际企业级工作流中Text2SQL任务的高级评估框架。它包含 600 个复杂的Text2SQL工作流问题，这些问题来自各种企业数据库用例。数据集包括来自实际数据应用程序的数据库，通常包含 1,000 多列，存储在云端或本地系统中，如 BigQuery、Snowflake 或 PostgreSQL。Spider 2.0 中的问题需要理解和搜索数据库元数据、方言文档和项目级代码库。挑战包括处理长上下文、执行复杂推理以及生成具有多种操作的多个 SQL 查询，通常超过 100 行。目前最先进的模型（如 GPT-4）仅解决了 6.0% 的问题，这凸显了数据集的难度以及对更高级、自主的基于 LLM 的代码代理的需求。

## 🌈 评测指标
- Execution Accuracy (EX) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - 定义：计算SQL执行结果正确的数量在数据集中的比例，结果存在高估的可能。

- Exact Match (EM) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - 定义：计算模型生成的SQL和标注SQL的匹配程度，结果存在低估的可能。

## 📦 库函数
- [mindsql](https://pypi.org/project/mindsql/)
  - MindSQL 是一个 Python RAG（检索增强生成）库，旨在仅使用几行代码来简化用户与其数据库之间的交互。 MindSQL 与 PostgreSQL、MySQL、SQLite 等知名数据库无缝集成，还通过扩展核心类，将其功能扩展到 Snowflake、BigQuery 等主流数据库。 该库利用 GPT-4、Llama 2、Google Gemini 等大型语言模型 (LLM)，并支持 ChromaDB 和 Fais 等知识库。
- [PremSQL](https://github.com/premAI-io/premsql)
  - PremSQL 是一个轻量级库，旨在为自然语言到 SQL 应用程序提供模块化和可扩展的工具。这将帮助开发人员基于不同的数据库构建更可控的 RAG 解决方案。它旨在提供用于评估、微调、连接器和代理框架的工具。PremSQL 还提出了 [Prem-1B-SQL](https://huggingface.co/premai-io/prem-1B-SQL)，这是一个 1B 参数的文本到 SQL 模型，在 BirdBench 私有测试集上达到 51.54%。它非常轻量，适用于完全本地文本到 SQL 生成。
  
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

## 🔗 引用
如果您发现`Text2SQL`对您的研究或开发有用，请引用以下<a href="https://arxiv.org/abs/2406.11434" target="_blank">论文</a>：

```bibtex
@misc{zhou2024dbgpthub,
      title={DB-GPT-Hub: Towards Open Benchmarking Text-to-SQL Empowered by Large Language Models}, 
      author={Fan Zhou and Siqiao Xue and Danrui Qi and Wenhui Shi and Wang Zhao and Ganglin Wei and Hongyang Zhang and Caigai Jiang and Gangwei Jiang and Zhixuan Chu and Faqiang Chen},
      year={2024},
      eprint={2406.11434},
      archivePrefix={arXiv},
      primaryClass={id='cs.DB' full_name='Databases' is_active=True alt_name=None in_archive='cs' is_general=False description='Covers database management, datamining, and data processing. Roughly includes material in ACM Subject Classes E.2, E.5, H.0, H.2, and J.1.'}
}
```

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
