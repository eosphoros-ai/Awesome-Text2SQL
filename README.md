# **Awesome Text2SQL**🎉🎉🎉

[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/eosphoros-ai/Awesome-Text2SQL/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)

**English** | [**中文版**](README.zh.md)

Curated tutorials and resources for Large Language Models, Text2SQL, and more.

## 🌱 How to Contribute
We warmly welcome contributions from everyone, whether you've found a typo, a bug, have a suggestion, or want to share a resource related to LLM+Text2SQL. For detailed guidelines on how to contribute, please see our [CONTRIBUTING.md](CONTRIBUTING.md) file.

## 🔔 Leaderboard


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


## 📜 Contents
- [**Awesome Text2SQL**🎉🎉🎉](#awesome-text2sql)
  - [🌱 How to Contribute](#-how-to-contribute)
  - [📜 Contents](#-contents)
  - [👋 Introduction](#-introduction)
  - [📖 Survey](#-survey)
  - [💬 Classic Model](#-classic-model)
  - [🔥 Base Model](#-base-model)
  - [💡 Fine-tuning](#-fine-tuning)
  - [💪 Dataset](#-dataset)
  - [🌈 Evaluation Index](#-evaluation-index)
  - [🔧 Practice Project](#-practice-project)
  - [🤝 Friendship Links](#-friendship-links)

## 👋 Introduction
- Text-to-SQL (or Text2SQL), as the name implies, is to convert text into SQL. A more academic definition is to convert natural language problems in the database field into structured query languages ​​that can be executed in relational databases. Therefore, Text-to-SQL can also be abbreviated as NL2SQL.
  - Input: natural language questions, such as "*Query the relevant information of the table t_user, and the results are sorted in descending order by id, and only the first 10 data are kept.*"
  - Output: SQL, such as "*SELECT * FROM t_user ORDER BY id DESC LIMIT 10*"

## 📖 Survey
- (2023-International Conference on Very Large Data Bases, VLDB, CCF-A）A survey on deep learning approaches for text-to-SQL [[paper](https://link.springer.com/article/10.1007/s00778-022-00776-8)]
- (2022-IEEE Transactions on Knowledge and Data Engineering, TKDE, CCF-A) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
- (2022-International Conference on Computational Linguistics, COLOING, CCF-B) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect [[paper](https://arxiv.org/pdf/2208.10099v1.pdf)]
- (2022-arXiv)Deep Learning Driven Natural Languages Text to SQL Query Conversion: A Survey [[paper](https://arxiv.org/pdf/2208.04415.pdf)]

## 💬 Classic Model
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

- Code LLama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023/08, Meta AI proposes Code LLama, based on Llama 2. Code Llama reaches state-of-the-art performance among open models on several code benchmarks. There are foundation models (Code Llama), Python specializations (Code Llama - Python), and instruction-following models,  with 7B, 13B and 34B parameters each.

- Qwen [[paper](https://qianwen-res.oss-cn-beijing.aliyuncs.com/QWEN_TECHNICAL_REPORT.pdf)] [[code](https://github.com/QwenLM/Qwen)] [[model](https://huggingface.co/Qwen)]
  - 2023/08, Alibaba Cloud proposes the 7b-parameter version of the large language model series Qwen-7B (abbr. Tongyi Qianwen), is pretrained on a large volume of data, including web texts, books, codes, etc, which has open sourced two models with Qwen-7B and Qwen-7B-Chat. 2023/09, Alibaba Cloud updated the Qwen-7B and Qwen-7B-Chat and open sourced Qwen-14B and Qwen-14B-Chat.

- Baichuan 2 [[code](https://github.com/baichuan-inc/Baichuan2)] [[model](https://huggingface.co/baichuan-inc)]
  - 2023/09, Baichuan Intelligent Technology proposes the new generation of open-source large language models Baichuan 2, trained on a high-quality corpus with 2.6 trillion tokens, which has base and chat versions for 7B and 13B, and a 4bits quantized version for the chat model.

- Phi-1.5 [[paper](https://arxiv.org/pdf/2309.05463.pdf)] [[model](https://huggingface.co/microsoft/phi-1_5)]
  - 2023/09, Microsoft Research proposes the open source language model phi-1.5, a Transformer with 1.3 billion parameters, which was trained using the same data sources as [phi-1](https://huggingface.co/microsoft/phi-1), augmented with a new data source that consists of various NLP synthetic texts. When assessed against benchmarks testing common sense, language understanding, and logical reasoning, phi-1.5 demonstrates a nearly state-of-the-art performance among models with less than 10 billion parameters.
 

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

- Spider [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider)] [[dataset](https://yale-lily.github.io/spider)]
  - 2018/09, Yale University proposes the Text-to-SQL dataset Spider with multiple databases, multiple tables, and single-round query. It is also recognized as the most difficult large-scale cross-domain evaluation list in the industry. It contains 10,181 natural language questions and 5,693 SQL statements. Involving more than 200 databases in 138 different fields, the difficulty level is divided into: easy, medium, difficult, and extremely difficult.

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

- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase)] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
  - 2021/08, Xi'an Jiaotong University and Microsoft propose the first cross-domain, multi-round Text-to-SQL Chinese dataset, which contains a list of 5459 multi-round questions and 17940 <query, SQL> binary groups.


- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)] [[dataset](https://bird-bench.github.io/)]
  - 2023/05, the University of Hong Kong and Alibaba propose a large-scale cross-domain dataset BIRD, which contains over 12,751 unique question-SQL pairs, 95 big databases with a total size of 33.4 GB. It also covers more than 37 professional domains, such as blockchain, hockey, healthcare and education, etc.


## 🌈 Evaluation Index
- Execution Accuracy (EX) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - Definition: Calculate the proportion of the correct number of SQL execution results in the data set, and the result may be overestimated.

- Exact Match (EM) [[paper](https://arxiv.org/pdf/2208.13629.pdf)]
  - Definition: Calculate the matching degree between the SQL generated by the model and the marked SQL, and the result may be underestimated.


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

