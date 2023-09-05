# Awesome Domain LLM

[![Awesome](https://camo.githubusercontent.com/64f8905651212a80869afbecbf0a9c52a5d1e70beab750dea40a994fa9a9f3c6/68747470733a2f2f617765736f6d652e72652f62616467652e737667)](https://github.com/luban-agi/awesome-Domain-LLM) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) 
![](https://img.shields.io/github/last-commit/luban-agi/Awesome-Domain-LLM?color=green)

自ChatGPT为代表的大语言模型（Large Language Model, LLM）出现以后，掀起了新一轮研究和应用浪潮，出现了许多包括LLaMA、ChatGLM、Baichuan、Qwen等在内的开源通用模型。
随后，来自不同领域的人们基于开源通用模型通过持续预训练/指令微调将其应用于垂直领域。
本项目旨在收集和梳理垂直领域的开源模型、数据集及评测基准。

欢迎大家贡献本项目未收录的开源模型、数据集、评测基准等，一起推动大模型赋能各行各业！

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

- [DoctorGLM](https://github.com/xionghonglin/DoctorGLM)
  ![](https://img.shields.io/github/stars/xionghonglin/DoctorGLM.svg?style=social)
  [[paper](https://arxiv.org/abs/2304.01097)]
  - 基于ChatGLM-6B的中文问诊模型，通过中文医疗对话数据集进行微调，实现了包括lora、p-tuningv2等微调及部署。

- [BenTsao (本草)](https://github.com/SCIR-HI/Huatuo-Llama-Med-Chinese)
  ![](https://img.shields.io/github/stars/SCIR-HI/Huatuo-Llama-Med-Chinese.svg?style=social)
  [[paper](https://arxiv.org/abs/2304.06975)]
  - 该项目开源了经过中文医学指令微调的大语言模型集，包括LLaMA、Alpaca-Chinese、Bloom、活字模型等。我们基于医学知识图谱以及医学文献，结合ChatGPT API构建了中文医学指令微调数据集，并以此对各种基模型进行了指令微调，提高了基模型在医疗领域的问答效果。
  
- [Med-ChatGLM](https://github.com/SCIR-HI/Med-ChatGLM)
  ![](https://img.shields.io/github/stars/SCIR-HI/Med-ChatGLM.svg?style=social)
  - 该项目开源了经过中文医学指令微调的ChatGLM-6B模型，微调数据与BenTsao相同。
    
- [BianQue (扁鹊)](https://github.com/scutcyr/BianQue)
  ![](https://img.shields.io/github/stars/scutcyr/BianQue.svg?style=social)
  - 该项目开源了生活空间健康大模型。结合当前开源的中文医疗问答数据集（MedDialog-CN、IMCS-V2、CHIP-MDCFNPC、MedDG、cMedQA2、Chinese-medical-dialogue-data），分析其中的单轮/多轮特性以及医生问询特性，结合自建的生活空间健康对话大数据，构建了千万级别规模的扁鹊健康大数据BianQueCorpus，基于扁鹊健康大数据BianQueCorpus，选择ChatGLM-6B作为初始化模型，经过全量参数的指令微调训练得到BianQue。
    
- [HuatuoGPT (华佗)](https://github.com/FreedomIntelligence/HuatuoGPT)
  ![](https://img.shields.io/github/stars/FreedomIntelligence/HuatuoGPT.svg?style=social)
  [[paper](https://arxiv.org/abs/2305.15075)]
  - 该项目开源了医疗大模型HuatuoGPT，包括基于Baichuan-7B训练得到的HuatuoGPT-7B和基于Ziya-LLaMA-13B-Pretrain-v1训练得到的HuatuoGPT-13B。

- [QiZhenGPT](https://github.com/CMKRG/QiZhenGPT)
  ![](https://img.shields.io/github/stars/CMKRG/QiZhenGPT.svg?style=social)
  - 该项目利用启真医学知识库构建的中文医学指令数据集，并基于此在Chinese-LLaMA-Plus-7B、CaMA-13B、ChatGLM-6B模型上进行指令精调，大幅提高了模型在中文医疗场景下效果。

- [ChatMed](https://github.com/michael-wzhu/ChatMed)
  ![](https://img.shields.io/github/stars/michael-wzhu/ChatMed.svg?style=social)
  - 该项目开源了中文医疗大模型ChatMed-Consult，以中文医疗在线问诊数据集ChatMed_Consult_Dataset的50w+在线问诊+ChatGPT回复作为训练集，基于LlaMA-7b采用LoRA微调得到。

- [ShenNong-TCM-LLM (神农)](https://github.com/michael-wzhu/ShenNong-TCM-LLM)
  ![](https://img.shields.io/github/stars/michael-wzhu/ShenNong-TCM-LLM.svg?style=social)
  - 该项目开源了中文中医药大模型ShenNong-TCM-LLM，以开源的中医药知识图谱为基础，采用以实体为中心的自指令方法，调用ChatGPT得到2.6w+中医药指令数据集ChatMed_TCM_Dataset，基于该数据集以LlaMA为底座，采用LoRA微调得到。

- [XrayGLM](https://github.com/WangRongsheng/XrayGLM)
  ![](https://img.shields.io/github/stars/WangRongsheng/XrayGLM.svg?style=social)
  - 该项目开源了中文多模态医学数据集及模型，其在医学影像诊断和多轮交互对话上显示出了非凡的潜力。

- [MedicalGPT](https://github.com/shibing624/MedicalGPT)
  ![](https://img.shields.io/github/stars/shibing624/MedicalGPT.svg?style=social)
  - 该项目开源了医疗大模型MedicalGPT，实现了包括增量预训练、有监督微调、RLHF(奖励建模、强化学习训练)和DPO(直接偏好优化)。

- [Sunsimiao (孙思邈)](https://github.com/thomas-yanxin/Sunsimiao)
  ![](https://img.shields.io/github/stars/thomas-yanxin/Sunsimiao.svg?style=social)
  - 该项目开源了中文医疗大模型Sunsimiao，该模型基于baichuan-7B和ChatGLM-6B底座模型在十万级高质量的中文医疗数据中微调而得。

- [CareLlama (关怀羊驼)](https://github.com/itsharex/CareLlama)
  ![](https://img.shields.io/github/stars/itsharex/CareLlama.svg?style=social)
  - 该项目开源了医疗大模型CareLlama，同时它收集了数十个公开可用的医疗微调数据集和开放可用的医疗大语言模型以促进医疗LLM快速发展。

- [DISC-MedLLM](https://github.com/FudanDISC/DISC-MedLLM)
  ![](https://img.shields.io/github/stars/FudanDISC/DISC-MedLLM.svg?style=social)
  [[paper](https://arxiv.org/abs/2308.14346)]
  - 该项目是由复旦大学发布的针对医疗健康对话式场景而设计的医疗领域大模型与数据集，该模型由DISC-Med-SFT数据集基于Baichuan-13B-Base指令微调得到，有效地对齐了医疗场景下的人类偏好，弥合了通用语言模型输出与真实世界医疗对话之间的差距。

- [PMC-LLaMA](https://github.com/chaoyi-wu/PMC-LLaMA)
  ![](https://img.shields.io/github/stars/chaoyi-wu/PMC-LLaMA.svg?style=social)
  [[paper](https://arxiv.org/abs/2304.14454)]
  - 该项目开源了医疗大模型PMC-LLaMA，包括预训练版本的MedLLaMA_13B和指令微调版本的PMC_LLaMA_13B。

- [ChatDoctor](https://github.com/Kent0n-Li/ChatDoctor)
  ![](https://img.shields.io/github/stars/Kent0n-Li/ChatDoctor.svg?style=social)
  [[paper](https://arxiv.org/abs/2303.14070)]
  - 该项目开源了医疗大模型ChatDoctor，在LLaMA的基础上训练得到。

- [MING (明医)](https://github.com/189569400/MedicalGPT-zh)
  ![](https://img.shields.io/github/stars/189569400/MedicalGPT-zh.svg?style=social)
  - 该项目开源了医疗大模型MING，基于bloomz-7b指令微调得到MING-7B，支持医疗问答、智能问诊等功能。

- [MeChat](https://github.com/qiuhuachuan/smile)
  ![](https://img.shields.io/github/stars/qiuhuachuan/smile.svg?style=social)
  - 该项目开源了中文心理健康支持对话大模型与数据集。模型由ChatGLM-6B LoRA 16-bit指令微调得到。数据集通过ChatGPT改写真实的心理互助QA为多轮的心理健康支持多轮对话，该数据集含有56k个多轮对话，其对话主题、词汇和篇章语义更加丰富多样，更加符合在长程多轮对话的应用场景。
  
- [SoulChat (灵心)](https://github.com/scutcyr/SoulChat)
  ![](https://img.shields.io/github/stars/scutcyr/SoulChat.svg?style=social)
  - 该项目开源了心理健康大模型灵心（SoulChat），该模型以ChatGLM-6B作为初始化模型，经过百万规模心理咨询领域中文长文本指令与多轮共情对话数据联合指令微调得到。

- [QiaoBan (巧板)](https://github.com/HIT-SCIR-SC/QiaoBan)
  ![](https://img.shields.io/github/stars/HIT-SCIR-SC/QiaoBan.svg?style=social)
  - 该项目开源了儿童情感对话大模型QiaoBan，基于开源通用大模型，使用通用域人机对话、单轮指令数据以及儿童情感陪伴对话数据进行指令微调，研发出适用于儿童情感陪伴的大模型。

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
  - 该项目开源了法律领域的指令微调数据和基于LLaMA训练的中文法律大模型Lawyer LLaMA。Lawyer LLaMA首先在大规模法律语料上进行了预训练，让它系统的学习中国的法律知识体系。在此基础上，借助ChatGPT收集了一批对中国国家统一法律职业资格考试客观题的分析和对法律咨询的回答，利用收集到的数据对模型进行指令微调，让模型习得将法律知识应用到具体场景中的能力。

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
  - 由浙江大学、阿里巴巴达摩院以及华院计算三家单位共同设计研发的法律大模型，基于Baichuan-7B进行了法律领域数据的二次预训练与指令微调，并设计了知识增强的推理流程。

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

- [MediaGPT](https://github.com/IMOSR/MediaGPT)
  ![](https://img.shields.io/github/stars/IMOSR/MediaGPT.svg?style=social)
  ![](https://img.shields.io/badge/自媒体-blue) 
  - 该项目开源了中文自媒体大模型，首先在大规模自媒体语料上进行连续预训练，系统地学习自媒体的知识体系。然后，借助ChatGPT收集了一批关于抖音运营、短视频创作、巨量千川投放、直播运营和直播话术技巧等领域知识问题的分析和回答，并利用这些数据对模型进行指令微调，使模型习得如何将自媒体知识应用到实际场景中。

- [EcomGPT](https://github.com/Alibaba-NLP/EcomGPT)
  ![](https://img.shields.io/github/stars/Alibaba-NLP/EcomGPT.svg?style=social)
  [[paper](https://arxiv.org/abs/2308.06966)]
  ![](https://img.shields.io/badge/电商-blue) 
  - 该项目开源了电商大模型，基于BLOOMZ在电商领域指令微调数据集EcomInstruct进行微调，在12个电商评测数据集上的人工评估超过ChatGPT。

- [StarGLM](https://github.com/Yu-Yang-Li/StarGLM)
  ![](https://img.shields.io/github/stars/Yu-Yang-Li/StarGLM.svg?style=social)
  ![](https://img.shields.io/badge/天文-blue) 
  - 该项目开源了天文大模型，整合司天工程相关的语料数据与知识库资料，训练得到天文大模型StarGLM，以期缓解大语言模型在天文通用知识和部分前沿变星领域的幻觉现象，为接下来可处理天文多模态任务、部署于望远镜阵列的观测Agent——司天大脑（数据智能处理）打下基础。

- [TransGPT (致远)](https://github.com/DUOMO/TransGPT)
  ![](https://img.shields.io/github/stars/DUOMO/TransGPT.svg?style=social)
  ![](https://img.shields.io/badge/交通-blue) 
  - 该项目开源了交通大模型，主要致力于在真实交通行业中发挥实际价值。它能够实现交通情况预测、智能咨询助手、公共交通服务、交通规划设计、交通安全教育、协助管理、交通事故报告和分析、自动驾驶辅助系统等功能。TransGPT作为一个通用常识交通大模型，可以为道路工程、桥梁工程、隧道工程、公路运输、水路运输、城市公共交通运输、交通运输经济、交通运输安全等行业提供通识常识。以此为基础，可以落脚到特定的交通应用场景中。

- [Mozi (墨子)](https://github.com/gmftbyGMFTBY/science-llm)
  ![](https://img.shields.io/github/stars/gmftbyGMFTBY/science-llm.svg?style=social)
  [[paper](https://github.com/gmftbyGMFTBY/science-llm/blob/main/asset/mozi_technical_report.pdf)]
  ![](https://img.shields.io/badge/论文-blue) 
  - 该项目开源了科技论文大模型，可以用于科技文献的问答和情感支持。

- [OpenBioMed](https://github.com/PharMolix/OpenBioMed)
  ![](https://img.shields.io/github/stars/PharMolix/OpenBioMed.svg?style=social)
  [[paper](https://arxiv.org/abs/2308.09442)]
  [[paper](https://arxiv.org/abs/2307.09484)]
  [[paper](https://arxiv.org/abs/2306.04371)]
  ![](https://img.shields.io/badge/生物医学-blue) 
  - 该项目开源了若干多模态生物医学大模型，包括多模态生物医药大模型BioMedGPT、多模态小分子基础模型DrugFM和MolFM、细胞表示学习模型CellLM等。
    
## 数据集

### 预训练数据集

### 微调数据集

## 评测基准

[![Star History Chart](https://api.star-history.com/svg?repos=luban-agi/Awesome-Domain-LLM&type=Date)](https://star-history.com/#luban-agi/Awesome-Domain-LLM&Date)

