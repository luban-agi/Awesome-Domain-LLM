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
  ![](https://img.shields.io/github/stars/HIT-SCIR-SC/QiaoBan.svg)
  - 该项目开源了儿童情感对话大模型，基于开源通用大模型，使用通用域人机对话、单轮指令数据以及儿童情感陪伴对话数据进行指令微调，研发出适用于儿童情感陪伴的大模型。

- [MediaGPT](https://github.com/IMOSR/MediaGPT)
  ![](https://img.shields.io/github/stars/IMOSR/MediaGPT.svg)
  - 该项目开源了中文自媒体大模型，首先在大规模自媒体语料上进行连续预训练，系统地学习自媒体的知识体系。然后，借助ChatGPT收集了一批关于抖音运营、短视频创作、巨量千川投放、直播运营和直播话术技巧等领域知识问题的分析和回答，并利用这些数据对模型进行指令微调，使模型习得如何将自媒体知识应用到实际场景中。

- [EcomGPT](https://github.com/Alibaba-NLP/EcomGPT)
  ![](https://img.shields.io/github/stars/Alibaba-NLP/EcomGPT.svg)
  [[paper](https://arxiv.org/abs/2308.06966)]
  - 该项目开源了电商大模型，基于BLOOMZ在电商领域指令微调数据集EcomInstruct进行微调，在12个电商评测数据集上的人工评估超过ChatGPT。

- [StarGLM](https://github.com/Yu-Yang-Li/StarGLM)
  ![](https://img.shields.io/github/stars/Yu-Yang-Li/StarGLM.svg)
  - 该项目开源了天文大模型，整合司天工程相关的语料数据与知识库资料，训练得到天文大模型StarGLM，以期缓解大语言模型在天文通用知识和部分前沿变星领域的幻觉现象，为接下来可处理天文多模态任务、部署于望远镜阵列的观测Agent——司天大脑（数据智能处理）打下基础。

- [TransGPT (致远)](https://github.com/DUOMO/TransGPT)
  ![](https://img.shields.io/github/stars/DUOMO/TransGPT.svg)
  - 简介：该项目开源了交通大模型，主要致力于在真实交通行业中发挥实际价值。它能够实现交通情况预测、智能咨询助手、公共交通服务、交通规划设计、交通安全教育、协助管理、交通事故报告和分析、自动驾驶辅助系统等功能。TransGPT作为一个通用常识交通大模型，可以为道路工程、桥梁工程、隧道工程、公路运输、水路运输、城市公共交通运输、交通运输经济、交通运输安全等行业提供通识常识。以此为基础，可以落脚到特定的交通应用场景中。

- [Mozi (墨子)](https://github.com/gmftbyGMFTBY/science-llm)
  ![](https://img.shields.io/github/stars/gmftbyGMFTBY/science-llm.svg)
  [[paper](https://github.com/gmftbyGMFTBY/science-llm/blob/main/asset/mozi_technical_report.pdf)]
  - 该项目开源了科技论文大模型，可以用于科技文献的问答和情感支持。
    
## 数据集

### 预训练数据集

### 微调数据集

## 评测基准

[![Star History Chart](https://api.star-history.com/svg?repos=luban-agi/Awesome-Domain-LLM&type=Date)](https://star-history.com/#luban-agi/Awesome-Domain-LLM&Date)

