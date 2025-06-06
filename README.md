# **Awesome Text2SQL**🎉🎉🎉

[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://img.shields.io/badge/Awesome-green.svg)](https://github.com/eosphoros-ai/Awesome-Text2SQL/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)


**English** | [**中文版**](README.zh.md) | [**Paper**](https://arxiv.org/abs/2406.11434)

Curated tutorials and resources for Large Language Models, Text2SQL, [Text2DSL](Text2DSL.md), [Text2API](Text2API.md), [Text2Vis](Text2Vis.md) and more.

## 🌱 How to Contribute
We warmly welcome contributions from everyone, whether you've found a typo, a bug, have a suggestion, or want to share a resource related to LLM+Text2SQL. For detailed guidelines on how to contribute, please see our [CONTRIBUTING.md](CONTRIBUTING.md) file.

## 🔔 Leaderboard

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

## 📜 Contents
- [**Awesome Text2SQL**🎉🎉🎉](#awesome-text2sql)
  - [🌱 How to Contribute](#-how-to-contribute)
  - [🔔 Leaderboard](#-leaderboard)
  - [📜 Contents](#-contents)
  - [👋 Introduction](#-introduction)
  - [📖 Survey](#-survey)
  - [💬 Classic Model](#-classic-model)
  - [🔥 Base Model](#-base-model)
  - [💡 Fine-tuning](#-fine-tuning)
  - [💪 Dataset](#-dataset)
  - [🌈 Evaluation Index](#-evaluation-index)
  - [📦 Libraries](#-libraries)
  - [🔧 Practice Project](#-practice-project)
  - [🔗 Citation](#-citation)
  - [🤝 Friendship Links](#-friendship-links)

## 👋 Introduction
- Text-to-SQL (or Text2SQL), as the name implies, is to convert text into SQL. A more academic definition is to convert natural language problems in the database field into structured query languages ​​that can be executed in relational databases. Therefore, Text-to-SQL can also be abbreviated as NL2SQL.
  - Input: natural language questions, such as "*Query the relevant information of the table t_user, and the results are sorted in descending order by id, and only the first 10 data are kept.*"
  - Output: SQL, such as "*SELECT * FROM t_user ORDER BY id DESC LIMIT 10*"

## 📖 Survey
- (2024-arXiv) Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL
[[paper](https://arxiv.org/pdf/2406.08426)]

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

## 💬 Classic Model
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

- (2024-NeurIPS, CCF-A) Towards Optimizing SQL Generation via LLM Routing
[[paper](https://arxiv.org/abs/2411.04319)]
[![](https://img.shields.io/badge/BIRD-yellow)](https://bird-bench.github.io/)

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

- (2023-AAAI 2023, CCF-A) **RESDSQL**: Decoupling Schema Linking and Skeleton Parsing for Text-to-SQL
[[paper](https://arxiv.org/pdf/2302.05965.pdf)]
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
[[paper](http://iir.ruc.edu.cn/~fanj/papers/sigmod2023-scprompt.pdf)]
[[code](https://github.com/ruc-datalab/SC-prompt)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/CoSQL-yellow)](https://arxiv.org/pdf/1909.05378.pdf)
[![](https://img.shields.io/badge/GenQuery-blue)](https://citeseerx.ist.psu.edu/document?repid=rep1&type=pdf&doi=1c9df99cce1903d34c53025e86e72331bbfbe08f)

- (2023-ICASSP, CCF-B) **T5-SR**: A Unified Seq-to-Seq Decoding Strategy for Semantic Parsing
[[paper](https://arxiv.org/pdf/2306.08368v1.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)

- (2022-ACL, CCF-A) **S<sup>2</sup>SQL**: Injecting Syntax to Question-Schema Interaction Graph Encoder for Text-to-SQL Parsers
[[paper](https://aclanthology.org/2022.findings-acl.99.pdf)]
[![](https://img.shields.io/badge/Spider-green)](https://yale-lily.github.io/spider)
[![](https://img.shields.io/badge/Spider--Syn-yellow)](https://arxiv.org/pdf/2106.01065.pdf)

- (2022-NAACL, CCF-B) **SeaD**: End-to-end Text-to-SQL Generation with Schema-aware Denoising
[[paper](https://arxiv.org/pdf/2105.07911v2.pdf)]
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


## 🔥 Base Model
- Llama [[paper](https://arxiv.org/pdf/2302.13971.pdf)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023/02, Meta AI proposes the open source LLM Llama, which has four scales: 7b, 13b, 33b, and 65b.

- ChatGLM [[paper](https://arxiv.org/pdf/2103.10360.pdf)] [[code](https://github.com/THUDM/ChatGLM-6B/blob/main/README.md)] [[model](https://huggingface.co/THUDM/chatglm-6b)]
  - 2023/03, Tsinghua University proposes the open bilingual language model ChatGLM, based on [General Language Model](https://github.com/THUDM/GLM) framework, with the specification of 7b.

- Alpaca [[paper](https://crfm.stanford.edu/2023/03/13/alpaca.html)] [[code](https://github.com/tatsu-lab/stanford_alpaca)] [[model](https://huggingface.co/tatsu-lab/alpaca-7b-wdiff/tree/main)]

  - 2023/03, Stanford University proposes Alpaca, an open source LLM fine-tuned based on the Llama 7b model. There are 1 specification of 7b, and the training is simpler and cheaper.

- Vicuna [[paper](https://lmsys.org/blog/2023-03-30-vicuna/)] [[code](https://github.com/lm-sys/FastChat)] [[model](https://huggingface.co/lmsys)]
  - 2023/03, UC Berkeley University, CMU and Stanford University propose Vicuna, an open souce LLM based on the  Llama model, has two specifications: 7b and 13b.

- WizardLM [[paper](https://arxiv.org/pdf/2304.12244.pdf)] [[code](https://github.com/nlpxucan/WizardLM)] [[model](https://huggingface.co/WizardLM)]
  - 2023/04, Peking University and Microsoft propose WizardLM, a LLM of evolutionary instructions, with three specifications of 7b, 13b, and 30b. 2023/06, They propose WizardMath, a LLM in the field of mathematics. 2023/08, They propose WizardCoder, a LLM in the field of code.

- Falcon [[paper](https://arxiv.org/pdf/2306.01116.pdf)] [[code](https://huggingface.co/tiiuae/falcon-180B)] [[model](https://huggingface.co/tiiuae)]
  - 2023/06, United Arab Emirates proposes Falcon, an open source LLM trained solely on refinedweb datasets, with four parameter specifications of 1b, 7b, 40b and 180b. It is worth noting that the performance on model 40B exceeds that of 65B LLaMA. 
  
- ChatGLM2[[paper](https://arxiv.org/pdf/2210.02414.pdf)] [[code](https://github.com/THUDM/ChatGLM2-6B/blob/main/README_EN.md)] [[model](https://huggingface.co/THUDM/chatglm2-6b)]
  - 2023/06, Tsinghua University proposes the second-generation version of ChatGLM，with the specification of 7b, which has stronger performance, longer context, more efficient inference and more open license.

- Baichuan-7b [[code](https://github.com/baichuan-inc/baichuan-7B)] [[model](https://huggingface.co/baichuan-inc/Baichuan-7B)]
  - 2023/06, Baichuan Intelligent Technology proposes the Baichuan-7B, an open-source, large-scale pre-trained language model based on Transformer architecture, which contains 7 billion parameters and trained on approximately 1.2 trillion tokens. It supports both Chinese and English languages with a context window length of 4096. 
  
- Baichuan-13b [[code](https://github.com/baichuan-inc/Baichuan-13B)] [[model](https://huggingface.co/baichuan-inc/Baichuan-13B-Base)]
  - 2023/07, Baichuan Intelligent Technology proposes the Baichuan-13B, an open-source, commercially available large-scale language model, following Baichuan-7B, which has two versions: pre-training (Baichuan-13B-Base) and alignment (Baichuan-13B-Chat).

- InternLM [[paper](https://github.com/InternLM/InternLM-techreport/blob/main/InternLM.pdf)] [[code](https://github.com/InternLM/InternLM/)] [[model](https://huggingface.co/internlm)]
  - 2023/07, Shanghai AI Laboratory and SenseTime propose the InternLM,  which has open-sourced a 7b and 20b parameter base models and chat models tailored for practical scenarios and the training system.

- Llama 2 [[paper](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023/07, Meta AI proposes the second-generation Llama series open-source LLM Llama 2. Compared with Llama 1, the training data is 40% more, and the context length is doubled. The model has four specifications: 7b, 13b, 34b, and 70b, but 34b is not open source. 

- Code Llama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023/08, Meta AI proposes Code LLama, based on Llama 2. Code Llama reaches state-of-the-art performance among open models on several code benchmarks. There are foundation models (Code Llama), Python specializations (Code Llama - Python), and instruction-following models,  with 7B, 13B and 34B parameters each. 2024/01, Meta AI open sourced CodeLlama-70b, CodeLlama-70b-Python and CodeLlama-70b-Instruct.

- Qwen [[paper](https://qianwen-res.oss-cn-beijing.aliyuncs.com/QWEN_TECHNICAL_REPORT.pdf)] [[code](https://github.com/QwenLM/Qwen)] [[model](https://huggingface.co/Qwen)]
  - 2023/08, Alibaba Cloud proposes the 7b-parameter version of the large language model series Qwen-7B (abbr. Tongyi Qianwen), is pretrained on a large volume of data, including web texts, books, codes, etc, which has open sourced two models with Qwen-7B and Qwen-7B-Chat. 2023/09, Alibaba Cloud updated the Qwen-7B and Qwen-7B-Chat and open sourced Qwen-14B and Qwen-14B-Chat. 2023/11, they open sourced Qwen-1.8B, Qwen-1.8B-Chat, Qwen-72B and Qwen-72B-Chat.

- Baichuan 2 [[paper](https://arxiv.org/pdf/2309.10305.pdf)]
[[code](https://github.com/baichuan-inc/Baichuan2)] [[model](https://huggingface.co/baichuan-inc)]
  - 2023/09, Baichuan Intelligent Technology proposes the new generation of open-source large language models Baichuan 2, trained on a high-quality corpus with 2.6 trillion tokens, which has base and chat versions for 7B and 13B, and a 4bits quantized version for the chat model.

- Phi-1.5 [[paper](https://arxiv.org/pdf/2309.05463.pdf)] [[model](https://huggingface.co/microsoft/phi-1_5)]
  - 2023/09, Microsoft Research proposes the open source language model phi-1.5, a Transformer with 1.3 billion parameters, which was trained using the same data sources as [phi-1](https://huggingface.co/microsoft/phi-1), augmented with a new data source that consists of various NLP synthetic texts. When assessed against benchmarks testing common sense, language understanding, and logical reasoning, phi-1.5 demonstrates a nearly state-of-the-art performance among models with less than 10 billion parameters. 2023/12, They propose [Phi-2](https://huggingface.co/microsoft/phi-2), a 2.7 billion-parameter language model that demonstrates outstanding reasoning and language understanding capabilities, showcasing state-of-the-art performance among base language models with less than 13 billion parameters. 

 - Mistral-7B [[paper](https://arxiv.org/pdf/2310.06825.pdf)]
    [[code](https://github.com/mistralai/mistral-src)] 
    [[model](https://huggingface.co/mistralai/Mistral-7B-v0.1)]
   - 2023/10, Mistral-AI company proposes the open source LLM Mistral 7B, a 7–billion-parameter language model engineered for superior performance and efficiency. Mistral 7B outperforms the best open 13B model (Llama 2) across all evaluated benchmarks, and the best released 34B model (Llama 1) in reasoning, mathematics, and code generation. They also provide a model fine-tuned to follow instructions, Mistral 7B – Instruct, that surpasses Llama 2 13B–chat model both on human and automated benchmarks. 2023/12，They propose the open source LLM Mixtral-8x7B, a pretrained generative Sparse Mixture of Experts, which outperforms Llama 2 70B on most benchmarks.

 - Deepseek [[paper](https://arxiv.org/pdf/2401.02954.pdf)]
    [[code](https://github.com/deepseek-ai/DeepSeek-LLM)] 
    [[model](https://huggingface.co/deepseek-ai)]
   - 2023/11, DeepSeek-AI company proposes the open source LLM deepseek, which has been trained from scratch on a vast dataset of 2 trillion tokens in both English and Chinese. Similarly, the deepseek LLM mainly has two categories: base and chat, with two parameter formats of 7b and 67b respectively. Data from its paper shows that deepSeek LLM 67b surpasses LLaMA-2 70b across a range of benchmarks, especially in the domains of code, mathematics, and reasoning. Furthermore, DeepSeek LLM 67B Chat exhibits superior performance compared to GPT-3.5.

 - MiniCPM [[paper](https://shengdinghu.notion.site/MiniCPM-c805a17c5c8046398914e47f0542095a)]
    [[code](https://github.com/OpenBMB/MiniCPM)] 
    [[model](https://huggingface.co/openbmb)]
   - 2024/02, ModelBest Inc. and TsinghuaNLP proposes the open source LLM MiniCPM, which is an End-Side LLM, with only 2.4B parameters excluding embeddings (2.7B in total). It is worth that MiniCPM has very close performance compared with Mistral-7B on open-sourced general benchmarks with better ability on Chinese, Mathematics and Coding after SFT. The overall performance exceeds Llama2-13B, MPT-30B, Falcon-40B, etc.

 - Mixtral-8x22B [[paper](https://mistral.ai/news/mixtral-8x22b/)] [[code](https://docs.mistral.ai/getting-started/open_weight_models/)] [[model](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1)]
   - 2024/04, Mistral AI proposed the latest open model Mixtral 8x22B. It sets a new standard for performance and efficiency within the AI community. It is a sparse Mixture-of-Experts (SMoE) model that uses only 39B active parameters out of 141B, offering unparalleled cost efficiency for its size.

 - Phi-3 [[paper](https://azure.microsoft.com/en-us/blog/introducing-phi-3-redefining-whats-possible-with-slms/)] [[model](https://huggingface.co/microsoft/Phi-3-mini-128k-instruct)]
   - 2024/04, Microsoft proposed the Phi-3 models, which are the most capable and cost-effective small language models (SLMs) available, outperforming models of the same size and next size up across a variety of language, reasoning, coding, and math benchmarks. Phi-3-mini is available in two context-length variants—4K and 128K tokens. It is the first model in its class to support a context window of up to 128K tokens, with little impact on quality. Phi-3-small (7B) and Phi-3-medium (14B) will be available in the Azure AI model catalog and other model gardens shortly.   

  - Llama 3 [[paper](https://ai.meta.com/blog/meta-llama-3/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
    - 2024/04, Meta AI proposed the third generation Llama series open source large model Llama 3. The model has 2 parameter specifications, 8b and 70b, with base and instruct versions respectively. Excitingly, Llama 3 models are a major leap over Llama 2 and establish a new state-of-the-art for LLM models at those scales.

  - Qwen-1.5-110B [[paper](https://qwenlm.github.io/blog/qwen1.5-110b/)] [[code](https://github.com/QwenLM/Qwen1.5)] [[model](https://huggingface.co/Qwen/Qwen1.5-110B)]
    - 2024/04, Alibaba Cloud proposed the first 100B+ model of the Qwen1.5 series, Qwen1.5-110B, which achieves comparable performance with Meta-Llama3-70B in the base model evaluation, and outstanding performance in the chat evaluation, including MT-Bench and AlpacaEval 2.0. Qwen1.5 is the beta version of Qwen2, which has 9 model sizes, including 0.5B, 1.8B, 4B, 7B, 14B, 32B, 72B, and 110B dense models, and an MoE model of 14B with 2.7B activated.
  
  - Qwen2 [[paper](https://qwenlm.github.io/blog/qwen2/)] [[code](https://github.com/QwenLM/Qwen2)] [[model](https://huggingface.co/collections/Qwen/qwen2-6659360b33528ced941e557f)]
    - 2024/06, Alibaba Cloud proposed the evolution from Qwen1.5 to Qwen2, which has 5 model sizes, including Qwen2-0.5B, Qwen2-1.5B, Qwen2-7B, Qwen2-57B-A14B, and Qwen2-72B. Qwen2-72B exhibits superior performance compared to leading models such as Llama-3-70B. Notably, it surpasses the performance of its predecessor, Qwen1.5-110B, despite having fewer parameters.

  - Llama 3.1  [[paper](https://ai.meta.com/blog/meta-llama-3-1/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
    - 2024/07, Meta AI proposed the Llama 3.1 405B, which is the first openly available model that rivals the top AI models when it comes to state-of-the-art capabilities in general knowledge, steerability, math, tool use, and multilingual translation. As part of this latest release, they’re introducing upgraded versions of the 8B and 70B models. These are multilingual and have a significantly longer context length of 128K, state-of-the-art tool use, and overall stronger reasoning capabilities. 

  - Qwen2.5 [[paper](https://arxiv.org/abs/2407.10671)] [[code](https://github.com/QwenLM/Qwen2.5)] [[model](https://huggingface.co/Qwen)]
    - 2024/09, Alibaba Cloud proposed the latest addition to the Qwen family: Qwen2.5, along with specialized models for coding, Qwen2.5-Coder, and mathematics, Qwen2.5-Math. All open-weight models are dense, decoder-only language models, available in various sizes, including: Qwen2.5(0.5B, 1.5B, 3B, 7B, 14B, 32B, and 72B), Qwen2.5-Coder (1.5B, 7B, and 32B on the way) and Qwen2.5-Math (1.5B, 7B, and 72B). They benchmarked their largest open-source model, Qwen2.5-72B-Instruct against leading open-source models like Llama-3.1-70B-Instrct and Mistral-Large-V2-Instruct and achieved the best results in multiple indicators. 
    


 - Llama 3.2  [[paper](https://ai.meta.com/blog/llama-3-2-connect-2024-vision-edge-mobile-devices/)] [[code](https://github.com/meta-llama/llama3)] [[model](https://huggingface.co/meta-llama)]
    - 2024/09, Meta AI proposed the Llama 3.2, which includes small and medium-sized vision LLMs (11B and 90B), and lightweight, text-only models (1B and 3B) that fit onto edge and mobile devices, including pre-trained and instruction-tuned versions. The Llama 3.2 1B and 3B models support context length of 128K tokens and are state-of-the-art in their class for on-device use cases like summarization, instruction following, and rewriting tasks running locally at the edge. These models are enabled on day one for Qualcomm and MediaTek hardware and optimized for Arm processors.
    
    

 ## 💡 Fine-tuning
- P-Tuning [[paper](https://arxiv.org/pdf/2103.10385.pdf)] [[code](https://github.com/THUDM/P-tuning)] 
  - 2021/03, Tsinghua University and others propose P-Tuning, a fine-tuning method for LLM, which uses trainable continuous prompt word embeddings to reduce the cost of fine-tuning.

- LoRA [[paper](https://arxiv.org/pdf/2106.09685.pdf)] [[code](https://github.com/microsoft/LoRA)] 
  - 2021/06, Microsoft proposes the Low-Rank Adaptation method for fine-tuning LLM by freezing the pre-training weights.

- P-Tuning V2 [[paper](https://arxiv.org/pdf/2110.07602.pdf)] [[code](https://github.com/THUDM/P-tuning-v2)] 
  - 2021/10, Tsinghua University proposes P-Tuning V2, an improved version of P-Tuning with better performance.

- RLHF [[paper](https://huggingface.co/blog/rlhf)] [[code](https://github.com/huggingface/blog/blob/main/zh/rlhf.md)] 
  - 2022/12, OpenAI uses the RLHF (Reinforcement Learning from Human Feedback) method to train ChatGPT, and uses human feedback signals to directly optimize the language model, with excellent performance.

- RRHF [[paper](https://arxiv.org/pdf/2304.05302.pdf)] [[code](https://github.com/GanjinZero/RRHF)] 
  - 2023/04, Alibaba proposes a novel learning paradigm called RRHF（Rank Responses to Align Language Models
  with Human Feedback without tears), which can be tuned as easily as fine-tuning and achieve a similar
  performance as PPO in HH dataset.

- QLoRA [[paper](https://arxiv.org/pdf/2305.14314.pdf)] [[code](https://github.com/artidoro/qlora)] 
  - 2023/05, Washington University proposes the qlora method, based on the frozen 4bit quantization model, combined with LoRA method training, which further reduces the cost of fine-tuning.

- RLTF [[paper](https://arxiv.org/pdf/2307.04349.pdf)] [[code](https://github.com/Zyq-scut/RLTF)] 
  - 2023/07, Tencent proposes RLTF（Reinforcement Learning from Unit Test Feedback), a novel online RL framework with unit test feedback of multi-granularity for refining code LLMs.

- RRTF [[paper](https://arxiv.org/pdf/2307.14936v1.pdf)]
  - 2023/07, Huawei proposes RRTF（Rank Responses to align Test&Teacher Feedback). Compared with RLHF, RRHF can efficiently align the output probabilities of a language model with human preferences, with only 1-2 models required during the tuning period, and it is simpler than PPO in terms of implementation, hyperparameter tuning, and training.

- RLAIF [[paper](https://arxiv.org/pdf/2309.00267.pdf)]
  - 2023/09, Google proposes RLAIF (RL from AI Feedback), a technique where preferences are labeled by an off-the-shelf LLM in lieu of humans. They find that the RLHF and RLAIF methods achieve the similar results on the task of summarization.


## 💪 Dataset
- WikiSQL [[paper](https://arxiv.org/pdf/1709.00103.pdf)] [[code](https://github.com/salesforce/WikiSQL)] [[dataset](https://github.com/salesforce/WikiSQL)]
  - 2017/09, Salesforce proposes a large Text-to-SQL dataset WikiSQL, the data comes from Wikipedia, which belongs to a single domain, contains 80,654 natural language questions, and 77,840 SQL statements. The form of SQL statements is relatively simple, and does not include sorting, grouping, and subqueries and other complex operations.

- Spider 1.0 [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider)] [[dataset](https://yale-lily.github.io/spider)]
  - 2018/09, Yale University proposes the Text-to-SQL dataset Spider with multiple databases, multiple tables, and single-round query. It is also recognized as the most difficult large-scale cross-domain evaluation list in the industry. It contains 10,181 natural language questions and 5,693 SQL statements. Involving more than 200 databases in 138 different fields, the difficulty level is divided into: easy, medium, difficult, and extremely difficult. 2024/02, Yale University has open sourced the test collection of Spider 1.0 leaderboard, and they will open source the Spider 2.0 data set in March.

- SParC [[paper](https://arxiv.org/pdf/1906.02285.pdf)] [[code](https://github.com/taoyds/sparc)] [[dataset](https://drive.google.com/uc?export=download&id=1Uu7NMHTR1tdQw1t7bAuM7OPU4LElVKfg)]
  - 2019/06, Yale University proposes a large dataset SParC for complex, cross-domain, and context-dependent(multi-turn) semantic parsing and text-to-SQL task, which consists of 4,298 coherent question sequences (12k+ unique individual questions annotated with SQL queries annotated by 14 Yale students), obtained from user interactions with 200 complex databases over 138 domains.

- CSpider [[paper](https://arxiv.org/pdf/1909.13293.pdf)] [[code](https://github.com/taolusi/chisp)] [[dataset](https://drive.google.com/drive/folders/1TxCUq1ydPuBdDdHF3MkHT-8zixluQuLa?usp=sharing)]
  - 2019/09, Westlake University propposes a large Chinese dataset CSpider for complex and cross-domain semantic parsing and text-to-SQL task, translated from Spider by 2 NLP researchers and 1 computer science student, which consists of 10,181 questions and 5,693 unique complex SQL queries on 200 databases with multiple tables covering 138 different domains. 

- CoSQL [[paper](https://arxiv.org/pdf/1909.05378.pdf)] [[code](https://yale-lily.github.io/cosql)] [[dataset](https://yale-lily.github.io/cosql)]
  - 2019/09, Yale University and Salesforce Research propose a cross-domain database CoSQL, which consists of 30k+ turns plus 10k+ annotated SQL queries, obtained from a Wizard-of-Oz (WOZ) collection of 3k dialogues querying 200 complex DBs spanning 138 domains.
  
- TableQA [[paper](https://arxiv.org/pdf/2006.06434.pdf)] [[dataset](https://www.luge.ai/#/luge/dataDetail?id=12)]
  - 2020/06, Zhuiyi Technology proposes a large-scale cross-domain Natural Language to SQL dataset TableQA in Chinese language consisting 64,891 questions and 20,311 unique SQL queries on over 6,000 tables.
  
- DuSQL [[paper](https://aclanthology.org/2020.emnlp-main.562.pdf)] [[dataset](https://www.luge.ai/#/luge/dataDetail?id=13)]
  - 2020/11, Baidu proposes a larges-scale and pragmatic Chinese dataset DuSQL for the cross-domain text-toSQL task, containing 200 databases, 813 tables, and 23,797 question/SQL pairs. 

- KaggleDBQA [[paper](https://arxiv.org/abs/2106.11455)] [[code](https://github.com/Chia-Hsuan-Lee/KaggleDBQA/)] [[dataset](https://github.com/Chia-Hsuan-Lee/KaggleDBQA/tree/main?tab=readme-ov-file#Data-Format)]
  - 2021/06, University of Washington and Microsoft Research propose KaggleDBQA, a cross-domain evaluation dataset of real Web databases with domain-specific data types, original formatting, and unrestricted questions. It includes 272 examples across 8 databases, with an average of 2.25 tables per database. The dataset is notable for its real-world data sources, natural question authoring environments, and database documentation with rich domain knowledge. Key statistics: 8.7% WHERE clauses, 73.5% VAL, 24.6% SELECT, and 6.8% NON-SELECT.
  
- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase)] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
  - 2021/08, Xi'an Jiaotong University and Microsoft propose the first cross-domain, multi-round Text-to-SQL Chinese dataset, which contains a list of 5459 multi-round questions and 17940 <query, SQL> binary groups.


- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)] [[dataset](https://bird-bench.github.io/)]
  - 2023/05, the University of Hong Kong and Alibaba propose a large-scale cross-domain dataset BIRD, which contains over 12,751 unique question-SQL pairs, 95 big databases with a total size of 33.4 GB. It also covers more than 37 professional domains, such as blockchain, hockey, healthcare and education, etc.


- BIRD-SQL Mini-Dev [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/bird-bench/mini_dev)] [[dataset](https://bird-bench.github.io/)]
  - 2024/06, the collaboration between the University of Hong Kong and Alibaba continues with the release of BIRD-SQL Mini-Dev, a lite version of their development dataset designed for efficient and cost-effective SQL model testing. This dataset compiles 500 high-quality text2SQL pairs from 11 distinct databases and supports both MySQL and PostgreSQL formats. It features the introduction of two new evaluation metrics: the Reward-based Valid Efficiency Score (R-VES) and the Soft F1-Score, both currently in beta and specifically developed to enhance the accuracy and efficiency of text-to-SQL models in a development setting.

- Spider 2.0 [[paper](https://spider2-sql.github.io/)] [[code](https://github.com/xlang-ai/Spider2)] [[dataset](https://github.com/xlang-ai/Spider2)]
  - 2024/08, Spider 2.0, proposed by XLang AI, serves as an advanced evaluation framework for text-to-SQL tasks within real-world enterprise-level workflows. It contains 600 complex text-to-SQL workflow problems, derived from various enterprise database use cases. The dataset includes databases sourced from actual data applications, often containing over 1,000 columns, and stored in cloud or local systems like BigQuery, Snowflake, or PostgreSQL. Problems in Spider 2.0 require understanding and searching through database metadata, dialect documentation, and project-level codebases. The challenges include processing long contexts, performing intricate reasoning, and generating multiple SQL queries with diverse operations, often exceeding 100 lines. Current state-of-the-art models, like GPT-4, solve only 6.0% of the questions, highlighting the dataset's difficulty and the need for more advanced, autonomous LLM-based code agents.

## 🌈 Evaluation Index
- Execution Accuracy (EX) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - Definition: Calculate the proportion of the correct number of SQL execution results in the data set, and the result may be overestimated.

- Exact Match (EM) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - Definition: Calculate the matching degree between the SQL generated by the model and the marked SQL, and the result may be underestimated.

## 📦 Libraries
- [mindsql](https://pypi.org/project/mindsql/)
  - MindSQL is a Python RAG (Retrieval-Augmented Generation) Library designed to streamline the interaction between users and their databases using just a few lines of code. With seamless integration for renowned databases such as PostgreSQL, MySQL, and SQLite, MindSQL also extends its capabilities to major databases like Snowflake and BigQuery by extending the core class. The library utilizes large language models (LLM) like GPT-4, Llama 2, Google Gemini, and supports knowledge bases like ChromaDB and Fais

- [PremSQL](https://github.com/premAI-io/premsql)
  - PremSQL is a lightweight library that aims to provide modular and extendible tools for natural language to SQL applications. This would help developers build more controllable RAG solutions based on different databases. It seeks to offer toolings for evaluation, fine-tuning, connectors, and agentic frameworks. PremSQL also comes up with [Prem-1B-SQL](https://huggingface.co/premai-io/prem-1B-SQL) a 1B parameter Text to SQL model with 51.54 % on BirdBench private test set. It is super light weight and works for fully local text to SQL generation.  

## 🔧 Practice Project
- [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) 
[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/DB-GPT-Hub?style=social)](https://github.com/eosphoros-ai/DB-GPT-Hub/stargazers)
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/DB-GPT-Hub?color=green)
  - The eosphoros organization proposes an open source project focusing on Text-to-SQL fine-tuning based on LLM, including large-scale model download, dataset preprocessing, fine-tuning technologies such as LoRA and QLoRA, model prediction, model evaluation and other steps.

- [sqlcoder](https://github.com/defog-ai/sqlcoder)
[![GitHub Repo stars](https://img.shields.io/github/stars/defog-ai/sqlcoder?style=social)](https://github.com/defog-ai/sqlcoder/stargazers)
![last commit](https://img.shields.io/github/last-commit/defog-ai/sqlcoder?color=green)
  - The Defog organization proposes an advanced Text-to-SQL LLM, which has outstanding performance and is better than GPT3.5, wizardcoder and starcoder, etc., second only to GPT4.

- [modal_finetune_sql](https://github.com/run-llama/modal_finetune_sql)
[![GitHub Repo stars](https://img.shields.io/github/stars/run-llama/modal_finetune_sql?style=social)](https://github.com/run-llama/modal_finetune_sql/stargazers)
![last commit](https://img.shields.io/github/last-commit/run-llama/modal_finetune_sql?color=green)
  - This project is based on the LLaMa 2 7b model for Text-to-SQL fine-tuning, which includes a complete training, fine-tuning, and evaluation process.

- [LLaMA-Efficient-Tuning](https://github.com/hiyouga/LLaMA-Efficient-Tuning) 
  [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Efficient-Tuning?style=social)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/stargazers)
  ![last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning?color=green)
  - Easy-to-use LLM fine-tuning framework (LLaMA-2, BLOOM, Falcon, Baichuan, Qwen, Chat

- [Datrics Text2SQL](https://github.com/datrics-ai/text2sql)
[![GitHub Repo stars](https://img.shields.io/github/stars/datrics-ai/text2sql?style=social)](https://github.com/datrics-ai/text2sql/stargazers)
![last commit](https://img.shields.io/github/last-commit/datrics-ai/text2sql?color=green)
  - Datrics Text2SQL is an open-source framework that uses a tuned RAG pipeline to generate SQL queries from natural language. It focuses on accurate schema retrieval, resolving ambiguous documentation, and improving generalization on real-world queries.

## 🔗 Citation
 If you find `Text2SQL` useful for your research or development, please cite the following <a href="https://arxiv.org/abs/2406.11434" target="_blank">paper</a>:

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

## 🤝 Friendship Links
- [eosphoros](https://github.com/eosphoros-ai)
[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai?style=social)](https://github.com/eosphoros-ai)
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/DB-GPT?color=green)
  - They are a team of technology enthusiasts from internet companies and NLP graduate students who are passionate about open source projects. Their focus is on developing solutions that protect the privacy and security of databases and large language models. Their aim is to ensure that the abilities of these models remain absolutely private, secure, and under control.

- [Awesome-AIGC-Tutorials](https://github.com/luban-agi/Awesome-AIGC-Tutorials)
  [![GitHub Repo stars](https://img.shields.io/github/stars/luban-agi/Awesome-AIGC-Tutorials?style=social)](https://github.com/luban-agi/Awesome-AIGC-Tutorials/stargazers)
  ![last commit](https://img.shields.io/github/last-commit/luban-agi/Awesome-AIGC-Tutorials?color=green)
  - Awesome AIGC Tutorials houses a curated collection of tutorials and resources spanning across Large Language Models, AI Painting, and related fields. Discover in-depth insights and knowledge catered for both beginners and advanced AI enthusiasts.

  [![Star History Chart](https://api.star-history.com/svg?repos=eosphoros-ai/Awesome-Text2SQL&type=Date)](https://star-history.com/#eosphoros-ai/Awesome-Text2SQL)

