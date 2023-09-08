# **Awesome Text2SQL**🎉🎉🎉


[![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![GitHub Repo forks](https://img.shields.io/github/forks/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/eosphoros-ai/Awesome-Text2SQL/)
[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/eosphoros-ai/Awesome-Text2SQL/) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![](https://img.shields.io/github/last-commit/eosphoros-ai/Awesome-Text2SQL?color=green)


[**English**](README.md) | **中文版**

这里收集了针对大型语言模型、Text2SQL 等的精选教程和资源。

## 📜 目录
- [👋 简介](#-简介)
- [📖 综述](#-综述)
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


## 🔥 基础模型
- Llama [[paper](https://arxiv.org/pdf/2302.13971.pdf)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023年2月，Meta AI提出开源大模型Llama，有7b、13b、33b、65b共4种规模。

- Alpaca [[paper](https://crfm.stanford.edu/2023/03/13/alpaca.html)] [[code](https://github.com/lm-sys/FastChat)] [[model](https://huggingface.co/lmsys)]
  - 2023年3月，斯坦福大学提出基于Llama 7b模型微调的开源大模型Alpaca，有7b共1种规格，训练更简单和便宜。

- Vicuna [[paper](https://lmsys.org/blog/2023-03-30-vicuna/)] [[code](https://github.com/tatsu-lab/stanford_alpaca)] [[model](https://github.com/tatsu-lab/stanford_alpaca)]
  - 2023年3月，UC伯克利大学联合CMU、斯坦福大学提出的开源大模型Vicuna，有7b、13b共2种规格。

- WizardLM [[paper](https://arxiv.org/pdf/2304.12244.pdf)] [[code](https://github.com/nlpxucan/WizardLM)] [[model](https://huggingface.co/WizardLM)]
  - 2023年4月，北京大学和微软提出进化指令大模型WizardLM，有7b、13b、30b共3种规格，2023年6月，提出了数学领域的大模型WizardMath，2023年8月提出了代码领域的大模型WizardCoder。

- Llama 2 [[paper](https://ai.meta.com/research/publications/llama-2-open-foundation-and-fine-tuned-chat-models/)] [[code](https://github.com/facebookresearch/llama)] [[model](https://huggingface.co/meta-llama)]
  - 2023年7月，Meta AI提出第二代Llama系列开源大模型Llama 2，和Llama 1相比，训练数据多40%，上下文长度翻倍，模型有7b、13b、34b、70b共4种规格，但是34b没有开源。

- Code LLama [[paper](https://arxiv.org/pdf/2308.12950.pdf)] [[code](https://github.com/facebookresearch/codellama)] [[model](https://huggingface.co/codellama)]
  - 2023年8月，Meta AI 在 Llama 2 的基础上提出 Code LLama。Code Llama 在多个代码基准测试中达到了开放模型中最先进的性能。有基础模型 (Code Llama)、Python 专业化 (Code Llama - Python) 和指令跟踪模型（instruction-following models），每个模型都有 7B、13B 和 34B 参数。


 ## 💡 微调
- P-Tuning [[paper](https://arxiv.org/pdf/2103.10385.pdf)] [[code](https://github.com/THUDM/P-tuning)] 
  - 2021年3月，清华大学等提出了针对大模型微调方法P-Tuning，采用可训练的连续提示词嵌入，降低了微调成本。

- LoRA [[paper](https://arxiv.org/pdf/2106.09685.pdf)] [[code](https://github.com/microsoft/LoRA)] 
  - 2021年6月，微软提出的针对大模型微调的Low-Rank Adaptation（LoRA）方法，冻结预训练权重。

- P-Tuning V2 [[paper](https://arxiv.org/pdf/2110.07602.pdf)] [[code](https://github.com/THUDM/P-tuning-v2)] 
  - 2021年10月，清华大学提出了P-Tuning的改进版本P-Tuning V2，性能更优。

- RLHF [[paper](https://huggingface.co/blog/rlhf)] [[code](https://github.com/huggingface/blog/blob/main/zh/rlhf.md)] 
  - 2022年12月，OpenAI使用RLHF方法训练ChatGPT，利用人类反馈信号直接优化语言模型，表现优异。

- QLoRA [[paper](https://arxiv.org/pdf/2305.14314.pdf)] [[code](https://github.com/artidoro/qlora)] 
  - 2023年5月，华盛顿大学基于冻结的4bit量化模型，结合LoRA方法训练，进一步降低了微调门槛。


## 💪 数据集
- WikiSQL [[paper](https://arxiv.org/pdf/1709.00103.pdf)] [[code](https://github.com/salesforce/WikiSQL)] [[dataset](https://github.com/salesforce/WikiSQL)]
  - 2017年9月，Salesforce提出的一个大型的Text-to-SQL数据集，数据来源于Wikipedia，属于单领域，包含了80654个自然语言问题，77840个SQL语句，SQL语句形式比较简单，不包含排序、分组、子查询等复杂操作。

- Spider [[paper](https://arxiv.org/pdf/1809.08887.pdf)] [[code](https://github.com/taoyds/spider)] [[dataset](https://yale-lily.github.io/spider)]
  - 2018年9月，耶鲁大学提出的多数据库、多表、单轮查询的Text-to-SQL数据集，也是业界公认难度最大的大规模跨领域评测榜单，包含了10181个自然语言问题，5693个SQL语句，涉及138个不同领域的200多个数据库，难易程度分为：简单、中等、困难、特别困难。

- CoSQL [[paper](https://arxiv.org/pdf/1909.05378.pdf)] [[code](https://yale-lily.github.io/cosql)] [[dataset](https://yale-lily.github.io/cosql)]
  - 2019/09, 耶鲁大学和Salesforce Research提出了一种跨域数据库CoSQL，它由30k+轮次和10k+带注释的SQL查询组成，这些查询是从Wizard-of-Oz (WOZ)集合中获得的，该集合包含3k个对话，查询跨越 138个域的200个复杂数据库。
  

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
