# **Awesome Text2SQL**🎉🎉🎉

[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/eosphoros-ai/Awesome-Text2SQL/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)

**English** | [**中文版**](README.zh.md)

Curated tutorials and resources for Large Language Models, Text2SQL, and more.

## 📜 Contents
- [👋 Introduction](#-introduction)
- [📖 Survey](#-survey)
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

## 🔥 Base Model
- Llama [[paper](https://arxiv.org/pdf/2302.13971.pdf)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023/02, Meta AI proposes the open source LLM Llama, which has four scales: 7b, 13b, 33b, and 65b.

- Alpaca [[paper](https://crfm.stanford.edu/2023/03/13/alpaca.html)] [[code](https://github.com/lm-sys/FastChat)] [[model](https://huggingface.co/lmsys)]
  - 2023/03, Stanford University proposes Alpaca, an open source LLM fine-tuned based on the Llama 7b model. There are 1 specification of 7b, and the training is simpler and cheaper.

- Vicuna [[paper](https://lmsys.org/blog/2023-03-30-vicuna/)] [[code](https://github.com/tatsu-lab/stanford_alpaca)] [[model](https://github.com/tatsu-lab/stanford_alpaca)]
  - 2023/03, UC Berkeley University, CMU and Stanford University propose Vicuna, an open souce LLM based on the  Llama model, has two specifications: 7b and 13b.

- WizardLM [[paper](https://arxiv.org/pdf/2304.12244.pdf)] [[code](https://github.com/nlpxucan/WizardLM)] [[model](https://huggingface.co/WizardLM)]
  - 2023/04, Peking University and Microsoft propose WizardLM, a LLM of evolutionary instructions, with three specifications of 7b, 13b, and 30b. 2023/06, They propose WizardMath, a LLM in the field of mathematics. 2023/08, They propose WizardCoder, a LLM in the field of code.

- Llama 2 [[paper](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023/07, Meta AI proposes the second-generation Llama series open-source LLM Llama 2. Compared with Llama 1, the training data is 40% more, and the context length is doubled. The model has four specifications: 7b, 13b, 34b, and 70b, but 34b is not open source. 

- Code LLama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023/08, Meta AI proposes Code LLama, based on Llama 2. Code Llama reaches state-of-the-art performance among open models on several code benchmarks. There are foundation models (Code Llama), Python specializations (Code Llama - Python), and instruction-following models,  with 7B, 13B and 34B parameters each.


 ## 💡 Fine-tuning
- P-Tuning [[paper](https://arxiv.org/pdf/2103.10385.pdf)] [[code](https://github.com/THUDM/P-tuning)] 
  - 2021/03, Tsinghua University and others propose P-Tuning, a fine-tuning method for LLM, which uses trainable continuous prompt word embeddings to reduce the cost of fine-tuning.

- LoRA [[paper](https://arxiv.org/pdf/2106.09685.pdf)] [[code](https://github.com/microsoft/LoRA)] 
  - 2021/06, Microsoft proposes the Low-Rank Adaptation method for fine-tuning LLM by freezing the pre-training weights.

- P-Tuning V2 [[paper](https://arxiv.org/pdf/2110.07602.pdf)] [[code](https://github.com/THUDM/P-tuning-v2)] 
  - 2021/10, Tsinghua University proposes P-Tuning V2, an improved version of P-Tuning with better performance.

- RLHF [[paper](https://huggingface.co/blog/rlhf)] [[code](https://github.com/huggingface/blog/blob/main/zh/rlhf.md)] 
  - 2022/12, OpenAI uses the RLHF method to train ChatGPT, and uses human feedback signals to directly optimize the language model, with excellent performance.

- QLoRA [[paper](https://arxiv.org/pdf/2305.14314.pdf)] [[code](https://github.com/artidoro/qlora)] 
  - 2023/05, Washington University proposes the qlora method, based on the frozen 4bit quantization model, combined with LoRA method training, which further reduces the cost of fine-tuning.


## 💪 Dataset
- WikiSQL [[paper](https://arxiv.org/pdf/1709.00103.pdf)] [[code](https://github.com/salesforce/WikiSQL)] [[dataset](https://github.com/salesforce/WikiSQL)]
  - 2017/09, Salesforce proposes a large Text-to-SQL dataset WikiSQL, the data comes from Wikipedia, which belongs to a single domain, contains 80,654 natural language questions, and 77,840 SQL statements. The form of SQL statements is relatively simple, and does not include sorting, grouping, and subqueries and other complex operations.

- Spider [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider))] [[dataset](https://yale-lily.github.io/spider)]
  - 2018/09, Yale University proposes the Text-to-SQL dataset Spider with multiple databases, multiple tables, and single-round query. It is also recognized as the most difficult large-scale cross-domain evaluation list in the industry. It contains 10,181 natural language questions and 5,693 SQL statements. Involving more than 200 databases in 138 different fields, the difficulty level is divided into: easy, medium, difficult, and extremely difficult.

- CoSQL [[paper](https://arxiv.org/pdf/1909.05378.pdf)] [[code](https://yale-lily.github.io/cosql)] [[dataset](https://yale-lily.github.io/cosql)]
  - 2019/09, Yale University and Salesforce Research propose a cross-domain database CoSQL, which consists of 30k+ turns plus 10k+ annotated SQL queries, obtained from a Wizard-of-Oz (WOZ) collection of 3k dialogues querying 200 complex DBs spanning 138 domains.
  

- CHASE [[paper](https://aclanthology.org/2021.acl-long.180.pdf)] [[code](https://github.com/xjtu-intsoft/chase))] [[dataset](https://github.com/xjtu-intsoft/chase/tree/page/data)]
  - 2021/08, Xi'an Jiaotong University and Microsoft propose the first cross-domain, multi-round Text-to-SQL Chinese dataset, which contains a list of 5459 multi-round questions and 17940 <query, SQL> binary groups.


- BIRD-SQL [[paper](https://arxiv.org/pdf/2305.03111.pdf)] [[code](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird))] [[dataset](https://bird-bench.github.io/)]
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
  - Easy-to-use LLM fine-tuning framework (LLaMA-2, BLOOM, Falcon, Baichuan, Qwen, ChatGLM2)



## 🤝 Friendship Links
- [eosphoros](https://github.com/eosphoros-ai)
[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai?style=social)](https://github.com/eosphoros-ai)
![last commit](https://img.shields.io/github/last-commit/eosphoros-ai/DB-GPT?color=green)
  - They are a team of technology enthusiasts from internet companies and NLP graduate students who are passionate about open source projects. Their focus is on developing solutions that protect the privacy and security of databases and large language models. Their aim is to ensure that the abilities of these models remain absolutely private, secure, and under control.

- [Awesome-AIGC-Tutorials](https://github.com/luban-agi/Awesome-AIGC-Tutorials)
[![GitHub Repo stars](https://img.shields.io/github/stars/luban-agi/Awesome-AIGC-Tutorials?style=social)](https://github.com/luban-agi/Awesome-AIGC-Tutorials/stargazers)
![last commit](https://img.shields.io/github/last-commit/luban-agi/Awesome-AIGC-Tutorials?color=green)
  - Awesome AIGC Tutorials houses a curated collection of tutorials and resources spanning across Large Language Models, AI Painting, and related fields. Discover in-depth insights and knowledge catered for both beginners and advanced AI enthusiasts.

