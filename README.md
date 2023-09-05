# Awesome Domain LLM

[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/luban-agi/awesome-Domain-LLM) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![](https://img.shields.io/github/last-commit/luban-agi/Awesome-Domain-LLM?color=green)

本项目旨在收集和梳理垂直领域的开源模型、数据集及评测基准。

## 目录

- [模型](#模型)
  - [医疗](#医疗)
  - [法律](#法律)
  - [金融](#金融)
  - [教育](#教育)
  - [其他](#其他)
- [数据集](#数据集)
  - [预训练数据集](#预训练数据集)
  - [微调数据集](#微调数据集)
- [评测基准](#评测基准)

## 模型

### 医疗

### 法律

- [LawGPT_zh (獬豸)](https://github.com/LiuHC0428/LAW-GPT)
  ![](https://img.shields.io/github/stars/LiuHC0428/LAW-GPT.svg?style=social)
  - 本项目开源的中文法律通用模型由ChatGLM-6B LoRA 16-bit指令微调得到。数据集包括现有的法律问答数据集和基于法条和真实案例指导的self-Instruct构建的高质量法律文本问答，提高了通用语言大模型在法律领域的表现，提高了模型回答的可靠性和专业程度。
    
- [LaWGPT](https://github.com/pengxiao-song/LaWGPT)
  ![](https://img.shields.io/github/stars/pengxiao-song/LaWGPT.svg?style=social)
  - 该系列模型在通用中文基座模型（如Chinese-LLaMA、ChatGLM等）的基础上扩充法律领域专有词表、大规模中文法律语料预训练，增强了大模型在法律领域的基础语义理解能力。在此基础上，构造法律领域对话问答数据集、中国司法考试数据集进行指令精调，提升了模型对法律内容的理解和执行能力。

- [LexiLaw](https://github.com/CSHaitao/LexiLaw)
  ![](https://img.shields.io/github/stars/CSHaitao/LexiLaw.svg?style=social)
  - LexiLaw是一个经过微调的中文法律大模型，它基于ChatGLM-6B架构，通过在法律领域的数据集上进行微调，使其在提供法律咨询和支持方面具备更高的性能和专业性。该模型旨在为法律从业者、学生和普通用户提供准确、可靠的法律咨询服务。无论是需要针对具体法律问题的咨询，还是对法律条款、案例解析、法规解读等方面的查询，LexiLaw都能够提供有益的建议和指导。

- [Lawyer LLaMA](https://github.com/AndrewZhe/lawyer-llama)
  ![](https://img.shields.io/github/stars/AndrewZhe/lawyer-llama.svg?style=social)
  [[paper](https://arxiv.org/abs/2305.15062)]
  - 开源了法律领域的指令微调数据和基于LLaMA训练的中文法律大模型Lawyer LLaMA。Lawyer LLaMA首先在大规模法律语料上进行了预训练，让它系统的学习中国的法律知识体系。在此基础上，借助ChatGPT收集了一批对中国国家统一法律职业资格考试客观题的分析和对法律咨询的回答，利用收集到的数据对模型进行指令微调，让模型习得将法律知识应用到具体场景中的能力。

- [HanFei (韩非)](https://github.com/siat-nlp/HanFei)
  ![](https://img.shields.io/github/stars/siat-nlp/HanFei.svg?style=social)
  - HanFei-1.0(韩非)是国内首个全参数训练的法律大模型，参数量7b，主要功能包括：法律问答、多轮对话、撰写文章、检索等。

- [ChatLaw](https://github.com/PKU-YuanGroup/ChatLaw)
  ![](https://img.shields.io/github/stars/PKU-YuanGroup/ChatLaw.svg?style=social)
  [[paper](https://arxiv.org/abs/2306.16092)]
  - 由北大开源的一系列法律大模型，使用大量法律新闻、法律论坛、法条、司法解释、法律咨询、法考题、判决文书等原始文本来构造对话数据，包括基于姜子牙-13B、Anima-33B训练而来的ChatLaw-13B和ChatLaw-33B。此外，还开源了ChatLaw-Text2Vec，使用93w条判决案例做成的数据集基于BERT训练了一个相似度匹配模型，可将用户提问信息和对应的法条相匹配。

- [Lychee (律知)](https://github.com/davidpig/lychee_law)
  ![](https://img.shields.io/github/stars/davidpig/lychee_law.svg?style=social)
  - 开源了中文司法领域大模型Law-GLM-10B，基于GLM-10B模型，在30GB中文法律数据上进行指令微调得到。

- [wisdomInterrogatory (智海-录问)](https://github.com/zhihaiLLM/wisdomInterrogatory)
  ![](https://img.shields.io/github/stars/zhihaiLLM/wisdomInterrogatory.svg?style=social)
  - 由浙江大学、阿里巴巴达摩院以及华院计算三家单位共同设计研发的法律大模型，基于Baichuan-7B进行了法律领域数据的二次预训练与指令微调，并设计了知识增强的推理流程。核心思想：以“普法共享和司法效能提升”为目标，从推动法律智能化体系入司法实践、数字化案例建设、虚拟法律咨询服务赋能等方面提供支持，形成数字化和智能化的司法基座能力。

### 金融

- [BBT-FinCUGE-Applications](https://github.com/ssymmetry/BBT-FinCUGE-Applications)
  ![](https://img.shields.io/github/stars/ssymmetry/BBT-FinCUGE-Applications.svg?style=social)
  [[paper](https://arxiv.org/abs/2302.09432)]
  - 该项目开源了中文金融领域语料库BBT-FinCorpus，知识增强型大模型BBT-FinT5及评测基准CFLEB。

- [Cornucopia (聚宝盆)](https://github.com/jerry1993-tech/Cornucopia-LLaMA-Fin-Chinese)
  ![](https://img.shields.io/github/stars/jerry1993-tech/Cornucopia-LLaMA-Fin-Chinese.svg?style=social)
  - 该项目基于公开和爬取的中文金融领域问答数据构建指令数据集，并在此基础上对LLaMA系模型进行了指令微调，提高了LLaMA在金融领域的问答效果。

- [XuanYuan (轩辕)](https://github.com/Duxiaoman-DI/XuanYuan)
  ![](https://img.shields.io/github/stars/Duxiaoman-DI/XuanYuan.svg?style=social)
  [[paper](https://arxiv.org/abs/2305.12002)]
  - 轩辕是国内首个开源的千亿级中文对话大模型，同时也是首个针对中文金融领域优化的千亿级开源对话大模型。轩辕在BLOOM-176B的基础上针对中文通用领域和金融领域进行了针对性的预训练与微调，它不仅可以应对通用领域的问题，也可以解答与金融相关的各类问题，为用户提供准确、全面的金融信息和建议。

- [PIXIU (貔貅)](https://github.com/chancefocus/PIXIU)
  ![](https://img.shields.io/github/stars/chancefocus/PIXIU.svg?style=social)
  [[paper](https://arxiv.org/abs/2306.05443)]
  - 该项目开源了金融领域指令微调数据集FIT，大模型FinMA及评测基准FLARE。

- [FinGPT](https://github.com/AI4Finance-Foundation/FinGPT)
  ![](https://img.shields.io/github/stars/AI4Finance-Foundation/FinGPT.svg?style=social)
  [[paper](https://arxiv.org/abs/2306.06031)]
  - 该项目开源了多个金融大模型，包括ChatGLM2-6B+LoRA和LLaMA2-7B+LoRA等金融大模型，收集了包括金融新闻、社交媒体、财报等中英文训练数据。

### 教育

- [桃李 (Taoli)](https://github.com/blcuicall/taoli)
  ![](https://img.shields.io/github/stars/blcuicall/taoli.svg?style=social)
  - 该项目开源了适用于国际中文教育领域的大模型，基于目前国际中文教育领域流通的500余册国际中文教育教材与教辅书、汉语水平考试试题以及汉语学习者词典等，构建了国际中文教育资源库。通过多种形式的指令构造了共计88000条的高质量国际中文教育问答数据集，并利用收集到的数据对模型进行指令微调，让模型习得将国际中文教育知识应用到具体场景中的能力。

- [EduChat](https://github.com/icalk-nlp/EduChat)
  ![](https://img.shields.io/github/stars/icalk-nlp/EduChat.svg?style=social)
  [[paper](https://arxiv.org/abs/2308.02773)]
  - 该项目开源了针对教育垂直领域的对话大模型，主要研究以预训练大模型为基底的教育对话大模型相关技术，融合多样化的教育垂直领域数据，辅以指令微调、价值观对齐等方法，提供教育场景下自动出题、作业批改、情感支持、课程辅导、高考咨询等丰富功能，服务于广大老师、学生和家长群体，助力实现因材施教、公平公正、富有温度的智能教育。

### 其他

- [QiaoBan (巧板)](https://github.com/HIT-SCIR-SC/QiaoBan)
  ![](https://img.shields.io/github/stars/HIT-SCIR-SC/QiaoBan.svg?style=social)
  - 该项目开源了儿童情感对话大模型，基于开源通用大模型，使用通用域人机对话、单轮指令数据以及儿童情感陪伴对话数据进行指令微调，研发出适用于儿童情感陪伴的大模型。

- [MediaGPT](https://github.com/IMOSR/MediaGPT)
  ![](https://img.shields.io/github/stars/IMOSR/MediaGPT.svg?style=social)
  - 该项目开源了中文自媒体大模型，首先在大规模自媒体语料上进行连续预训练，系统地学习自媒体的知识体系。然后，借助ChatGPT收集了一批关于抖音运营、短视频创作、巨量千川投放、直播运营和直播话术技巧等领域知识问题的分析和回答，并利用这些数据对模型进行指令微调，使模型习得如何将自媒体知识应用到实际场景中。

- [EcomGPT](https://github.com/Alibaba-NLP/EcomGPT)
  ![](https://img.shields.io/github/stars/Alibaba-NLP/EcomGPT.svg?style=social)
  [[paper](https://arxiv.org/abs/2308.06966)]
  - 该项目开源了电商大模型，基于BLOOMZ在电商领域指令微调数据集EcomInstruct进行微调，在12个电商评测数据集上的人工评估超过ChatGPT。

- [StarGLM](https://github.com/Yu-Yang-Li/StarGLM)
  ![](https://img.shields.io/github/stars/Yu-Yang-Li/StarGLM.svg?style=social)
  - 该项目开源了天文大模型，整合司天工程相关的语料数据与知识库资料，训练得到天文大模型StarGLM，以期缓解大语言模型在天文通用知识和部分前沿变星领域的幻觉现象，为接下来可处理天文多模态任务、部署于望远镜阵列的观测Agent——司天大脑（数据智能处理）打下基础。

- [TransGPT (致远)](https://github.com/DUOMO/TransGPT)
  ![](https://img.shields.io/github/stars/DUOMO/TransGPT.svg?style=social)
  - 该项目开源了交通大模型，主要致力于在真实交通行业中发挥实际价值。它能够实现交通情况预测、智能咨询助手、公共交通服务、交通规划设计、交通安全教育、协助管理、交通事故报告和分析、自动驾驶辅助系统等功能。TransGPT作为一个通用常识交通大模型，可以为道路工程、桥梁工程、隧道工程、公路运输、水路运输、城市公共交通运输、交通运输经济、交通运输安全等行业提供通识常识。以此为基础，可以落脚到特定的交通应用场景中。

- [Mozi (墨子)](https://github.com/gmftbyGMFTBY/science-llm)
  ![](https://img.shields.io/github/stars/gmftbyGMFTBY/science-llm.svg?style=social)
  [[paper](https://github.com/gmftbyGMFTBY/science-llm/blob/main/asset/mozi_technical_report.pdf)]
  - 该项目开源了科技论文大模型，可以用于科技文献的问答和情感支持。
    
## 数据集

### 预训练数据集

### 微调数据集

## 评测基准

[![Star History Chart](https://api.star-history.com/svg?repos=luban-agi/Awesome-Domain-LLM&type=Date)](https://star-history.com/#luban-agi/Awesome-Domain-LLM&Date)

