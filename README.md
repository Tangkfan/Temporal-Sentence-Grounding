# Awesome-Temporal-Video-Grounding

List of Temporal Video Grounding (TVG) papers.

The task is also usually referred to as:
- Temporal Sentence Grounding (TSG)
- Video Moment Retrieval (VMR)
- Temporal Activity Localization via Language Query (TALL)

TVG was initially introduced in 2017 as a novel task designed to localize specific moments in videos that are semantically relevant to given natural language queries.
Recent studies have started investigating techniques to augment the grounding capacity of large language models (LLMs), enabling them to better comprehend and temporally align visual information with natural language inputs.

# Content
- [Awesome-Temporal-Video-Grounding](#awesome-temporal-video-grounding)
- [Content](#content)
- [1 Survey](#1-survey)
- [2 Datasets](#2-datasets)
- [3 LLM for TVG](#3-llm-for-tvg)
  - [2023](#2023)
  - [2024](#2024)
  - [2025](#2025)
  - [2026](#2026)
- [4 Traditional TVG](#4-traditional-tvg)
  - [2017](#2017)
    - [Fully Supervised](#fully-supervised)
  - [2018](#2018)
    - [Fully Supervised](#fully-supervised-1)
    - [Weakly Supervised](#weakly-supervised)
  - [2019](#2019)
    - [Fully Supervised](#fully-supervised-2)
    - [Weakly Supervised](#weakly-supervised-1)
  - [2020](#2020)
    - [Fully Supervised](#fully-supervised-3)
    - [Weakly Supervised](#weakly-supervised-2)
  - [2021](#2021)
    - [Fully Supervised](#fully-supervised-4)
    - [Zero-Shot](#zero-shot)
  - [2022](#2022)
    - [Fully Supervised](#fully-supervised-5)
    - [Weakly Supervised](#weakly-supervised-3)
    - [Point-supervised/Glance](#point-supervisedglance)
  - [2023](#2023-1)
    - [Fully Supervised](#fully-supervised-6)
    - [Weakly Supervised](#weakly-supervised-4)
    - [Point-supervised/Glance](#point-supervisedglance-1)
    - [Zero-Shot](#zero-shot-1)
  - [2024](#2024-1)
    - [Fully Supervised](#fully-supervised-7)
    - [Weakly Supervised](#weakly-supervised-5)
  - [2025](#2025-1)
    - [Fully Supervised](#fully-supervised-8)
    - [Weakly Supervised](#weakly-supervised-6)
    - [Point-Supervised/Glance](#point-supervisedglance-2)


# 1 Survey
- [TPAMI'23] [Temporal Sentence Grounding in Videos: A Survey and Future Directions](https://ieeexplore.ieee.org/abstract/document/10075491). NTU 孙爱欣团队
- [ACM Comput. Surv.'23] [A Survey on Video Moment Localization](https://dl.acm.org/doi/abs/10.1145/3556537). 哈工大 聂礼强团队

# 2 Datasets
- [Charades-STA](https://prior.allenai.org/projects/charades): [VGG](https://github.com/TencentARC/UMT), [C3D](https://rochester.app.box.com/s/swu6rlqcdlebvwml8dyescmi7ra0owc5), [I3D](https://app.box.com/s/h0sxa5klco6qve5ahnz50ly2nksmuedw/folder/138545516584), [CLIP+SF](https://mailustceducn-my.sharepoint.com/personal/liuzhihang_mail_ustc_edu_cn/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fliuzhihang%5Fmail%5Fustc%5Fedu%5Fcn%2FDocuments%2FOpenSource%2FMESM%2Fdata&ga=1)
- [TACoS](https://www.coli.uni-saarland.de/projects/smile/page.php?id=tacos): [C3D](https://app.box.com/s/h0sxa5klco6qve5ahnz50ly2nksmuedw/folder/138544435150), [I3D](https://rochester.app.box.com/s/swu6rlqcdlebvwml8dyescmi7ra0owc5)
- [ActivityNet Captions](http://activity-net.org/download.html): [C3D](http://activity-net.org/challenges/2016/download.html)
- [QVHighlights](https://github.com/jayleicn/moment_detr/blob/main/data/README.md): [CLIP+SF](https://github.com/jayleicn/moment_detr)
- [Timelens-Bench](https://huggingface.co/datasets/TencentARC/TimeLens-Bench): Manually refined versions of Charades-STA, ActivityNet Captions and QVHighlights.
- [TimeLens-100K](https://huggingface.co/datasets/TencentARC/TimeLens-100K): High-quality training dataset.


# 3 LLM for TVG
## 2023
- [ACL] [Generating Structured Pseudo Labels for Noise-resistant Zero-shot Video Sentence Localization](https://aclanthology.org/2023.acl-long.794/). [[code](https://github.com/minghangz/SPL)]
- [ICCVW] [LLaViLo: Boosting Video Moment Retrieval via Adapter-Based Multimodal Modeling](https://openaccess.thecvf.com/content/ICCV2023W/CLVL/html/Ma_LLaViLo_Boosting_Video_Moment_Retrieval_via_Adapter-Based_Multimodal_Modeling_ICCVW_2023_paper.html). 
- [NeurIPS] [Self-Chained Image-Language Model for Video Localization and Question Answering](https://arxiv.org/abs/2305.06988). [[code](https://github.com/Yui010206/SeViLA)]
- [arXiv] [Grounding-Prompter: Prompting LLM with Multimodal Information for Temporal Sentence Grounding in Long Videos](https://arxiv.org/abs/2312.17117). 
- [arXiv] [LLM4VG: Large Language Models Evaluation for Video Grounding](https://arxiv.org/abs/2312.14206)


## 2024
- [ACL] [GroundingGPT: Language Enhanced Multi-modal Grounding Model](https://arxiv.org/abs/2401.06071). [[code](https://lzw-lzw.github.io/GroundingGPT.github.io/)]
- [CVPR] [VTimeLLM: Empower LLM to grasp video moments](https://openaccess.thecvf.com/content/CVPR2024/html/Huang_VTimeLLM_Empower_LLM_to_Grasp_Video_Moments_CVPR_2024_paper.html). [[code](https://github.com/huangb23/VTimeLLM)]
- [CVPR] [TimeChat: A time-sensitive multimodal large language model for long video understanding](https://openaccess.thecvf.com/content/CVPR2024/html/Ren_TimeChat_A_Time-sensitive_Multimodal_Large_Language_Model_for_Long_Video_CVPR_2024_paper.html). [[code](https://github.com/RenShuhuai-Andy/TimeChat)]
- [ECCV] [Training-free video temporal grounding using large-scale pre-trained models](https://link.springer.com/chapter/10.1007/978-3-031-73007-8_2). [[code](https://github.com/minghangz/TFVTG)]
- [EMNLP] [Efficient Temporal Extrapolation of Multimodal Large Language Models with Temporal Grounding Bridge](https://arxiv.org/abs/2402.16050). [[code](https://github.com/bigai-nlco/VideoTGB)]
- [NeurIPS] [SlowFocus: Enhancing fine-grained temporal understanding in video LLM](https://openreview.net/forum?id=FOkKndty5B). [[code](https://github.com/fudan-zvg/SlowFocus)]
- [arXiv] [The Surprising Effectiveness of Multimodal Large  Language Models for Video Moment Retrieval](https://arxiv.org/abs/2406.18113). [[code](https://github.com/sudo-Boris/mr-Blip)]
- [arXiv] [LLaVA-MR: Large Language-and-Vision Assistant for Video Moment Retrieval](https://arxiv.org/abs/2411.14505).
- [arXiv] [HawkEye: Training Video-Text LLMs for Grounding Text in Videos](https://arxiv.org/abs/2403.10228). [[code](https://github.com/yellow-binary-tree/HawkEye)]
- [arXiv] [Video LLMs for temporal reasoning in long videos](https://arxiv.org/abs/2412.02930)


## 2025
- [TMM] [ETC: Temporal boundary expand then clarify for weakly supervised video grounding with multimodal large language model](https://ieeexplore.ieee.org/abstract/document/10874219/). 
- [AAAI] [VTG-LLM: Integrating timestamp knowledge into video LLMs for enhanced video temporal grounding](https://ojs.aaai.org/index.php/AAAI/article/view/32341). [[code](https://github.com/gyxxyg/VTG-LLM)]
- [AAAI] [Zero-shot video moment retrieval via off-the-shelf multimodal large language models](https://arxiv.org/abs/2501.07972). 
- [ICLR] [TRACE: Temporal grounding video LLM via causal event modeling](https://arxiv.org/abs/2410.05643). [[code](https://github.com/gyxxyg/TRACE)]
- [ICLR] [TimeSuite: Improving MLLMs for long video understanding via grounded tuning](https://arxiv.org/abs/2410.19702). [[code](https://github.com/OpenGVLab/TimeSuite)]
- [CVPR] [SVLTA: Benchmarking vision-language temporal alignment via synthetic video situation](https://arxiv.org/abs/2504.05925). [[code](https://svlta-ai.github.io/SVLTA/)]
- [CVPR] [ReVisionLLM: Recursive vision-language model for temporal grounding in hour-long videos](https://arxiv.org/abs/2411.14901). [[code](https://github.com/Tanveer81/ReVisionLLM)]
- [CVPR] [Number it: Temporal grounding videos like flipping manga](https://arxiv.org/abs/2411.10332). [[code](https://github.com/yongliang-wu/NumPro)]
- [CVPR] [On the Consistency of Video Large Language Models in Temporal Comprehension](https://openaccess.thecvf.com/content/CVPR2025/html/Jung_On_the_Consistency_of_Video_Large_Language_Models_in_Temporal_CVPR_2025_paper.html). [[code](https://github.com/minjoong507/Consistency-of-Video-LLM)]
- [COLING] [Mitigating the discrepancy between video and text temporal sequences: A time-perception enhanced video grounding method for LLM](https://aclanthology.org/2025.coling-main.655/).
- [TIP'25] [Caption assisted multimodal large language model for video moment retrieval](https://ieeexplore.ieee.org/abstract/document/11206011).[[code](https://github.com/tjhd1475/CALCE)]
- [ICCV'25] [Enrich and Detect: Video Temporal Grounding  with Multimodal LLMs](https://openaccess.thecvf.com/content/ICCV2025/html/Pramanick_Enrich_and_Detect_Video_Temporal_Grounding_with_Multimodal_LLMs_ICCV_2025_paper.html).
- [ICCV'25] [Factorized Learning for Temporally Grounded Video-Language Models](https://arxiv.org/pdf/2512.24097) [[code](https://github.com/nusnlp/d2vlm)]
- [NeurIPS'25] [Uncertainty-quantified Rollout Policy Adaptation for Unlabelled Cross-domain Video Temporal Grounding](https://openreview.net/forum?id=RfNiN2rENM) [[code](https://lwpyh.github.io/URPA/)]
- [NeurIPS'25] [Time-R1: Post-training large vision language model for temporal video grounding](https://arxiv.org/abs/2503.13377). [[code](https://github.com/xiaomi-research/time-r1)]
- [arXiv] [Measure Twice, Cut Once: Grasping Video Structures and Event Semantics with LLMs for Video Temporal Localization](https://arxiv.org/abs/2503.09027). [[code](https://github.com/pangzss/MeCo)]
- [arXiv] [TimeRefine: Temporal grounding with time refining video LLM](https://arxiv.org/abs/2412.09601). [[code](https://github.com/SJTUwxz/TimeRefine)]
- [arXiv] [TimeZero: Temporal video grounding with reasoning-guided LVLM](https://arxiv.org/abs/2503.13377). [[code](https://github.com/www-Ye/TimeZero)]
- [arXiv] [MomentSeeker: A comprehensive benchmark and a strong baseline for moment retrieval within long videos](https://arxiv.org/abs/2502.12558).
- [arXiv] [VideoExpert: Augmented LLM for temporal-sensitive video understanding](https://arxiv.org/abs/2504.07519).
- [arXiv] [Universal Video Temporal Grounding with Generative Multi-modal Large Language Models](https://arxiv.org/abs/2506.18883).
- [arXiv] [VideoMind: A Chain-of-LoRA Agent for Long Video Reasoning](https://arxiv.org/abs/2503.13444). [[code](https://github.com/yeliudev/VideoMind?tab=readme-ov-file)]
- [arXiv] [Invert4TVG: A temporal video grounding framework with inversion tasks for enhanced action understanding](https://arxiv.org/abs/2508.07388).
- [arXiv] [VideoTG-R1: Boosting Video Temporal Grounding via Curriculum Reinforcement Learning on Reflected Boundary Annotations](https://arxiv.org/abs/2510.23397). [[code](https://github.com/ldong1111/VideoTG-R1)]
- [arXiv] [TempR1: Improving Temporal Understanding of MLLMs via Temporal-Aware Multi-Task Reinforcement Learning](https://arxiv.org/abs/2512.03963). 
- [arXiv] [TimeLens: Rethinking Video Temporal Grounding with Multimodal LLMs](https://arxiv.org/abs/2512.14698) [[website](https://timelens-arc-lab.github.io/)] [[code](https://github.com/TencentARC/TimeLens)]

## 2026
- [ECCV'26] [Parallelized Autoregressive Decoding for Omni-Modal Dense Video Captioning](https://arxiv.org/pdf/2607.02963) [[code](https://github.com/showlab/PadCaptioner)]

# 4 Traditional TVG
## 2017
首次提出TSG任务。
### <h3 id="fully-supervised-2017">Fully Supervised</h3>

**Proposal-based**
- [ICCV'17] [TALL: Temporal Activity Localization via Language Query](https://openaccess.thecvf.com/content_iccv_2017/html/Gao_TALL_Temporal_Activity_ICCV_2017_paper.html). 南加大 高继扬 [[code](https://github.com/jiyanggao/TALL)]
- [ICCV'17] [Localizing Moments in Video with Natural Language](https://openaccess.thecvf.com/content_iccv_2017/html/Hendricks_Localizing_Moments_in_ICCV_2017_paper.html). 伯克利 Lisa Anne Hendricks [[code](https://github.com/LisaAnne/LocalizingMoments)]

## 2018
### <h3 id="fully-supervised-2018">Fully Supervised</h3>
**Proposal-based**
- [EMNLP'18] [Temporally Grounding Natural Sentence in Video](https://aclanthology.org/D18-1015/). NUS Tat-Seng Chua团队
- [IJCAI'18] [Multi-modal Circulant Fusion for Video-to-Language and Backward](https://dl.acm.org/doi/abs/10.5555/3304415.3304561). 天大 韩亚洪团队
- [ACM MM'18] [Cross-modal Moment Localization in Videos](https://dl.acm.org/doi/abs/10.1145/3240508.3240549). 山东大学 聂礼强团队 [[code](https://acmmm18.wixsite.com/role)]
- [SIGIR'18] [Attentive Moment Retrieval in Videos](https://dl.acm.org/doi/abs/10.1145/3209978.3210003). 山东大学 聂礼强团队 [[code](https://sigir2018.wixsite.com/acrn)]

**Proposal-free**
- [AAAI'19] [Localizing Natural Language in Videos](https://ojs.aaai.org/index.php/AAAI/article/view/4827). 腾讯AI lab

### <h3 id="weakly-supervised-2018">Weakly Supervised</h3>
**Reconstruction-based**
- [NeurIPS'18] [Weakly Supervised Dense Event Captioning in Videos](https://proceedings.neurips.cc/paper/2018/hash/49af6c4e558a7569d80eee2e035e2bd7-Abstract.html). 清华 朱文武团队 [[code](https://github.com/ranjaykrishna/densevid_eval)]
    - 首次提出弱监督密集事件描述，在训练中涉及到了TSG问题

## 2019
### <h3 id="fully-supervised-2019">Fully Supervised</h3>
**Proposal-based**
- [AAAI'19] [Semantic Proposal for Activity Localization in Videos via Sentence Query](https://ojs.aaai.org/index.php/AAAI/article/view/4830). 复旦 姜育刚团队
- [CVPR'19] [MAN: Moment Alignment Network for Natural Language Moment Retrieval via Iterative Graph Adjustment](https://openaccess.thecvf.com/content_CVPR_2019/html/Zhang_MAN_Moment_Alignment_Network_for_Natural_Language_Moment_Retrieval_via_CVPR_2019_paper.html). UCSB Da Zhang
- [ACM MM'19] [Exploiting Temporal Relationships in Video Moment Localization with Natural Language](https://dl.acm.org/doi/abs/10.1145/3343031.3350879). UR 罗杰波团队 [[code](https://github.com/Sy-Zhang/TCMN-Release)]
- [NeurIPS'19] [Semantic Conditioned Dynamic Modulation for Temporal Sentence Grounding in Videos](https://proceedings.neurips.cc/paper_files/paper/2019/hash/6883966fd8f918a4aa29be29d2c386fb-Abstract.html). 清华 朱文武团队 [[code](https://github.com/yytzsy/SCDM)]
- [SIGIR'19] [Cross-Modal Interaction Networks for Query-Based Moment Retrieval in Videos](https://dl.acm.org/doi/abs/10.1145/3331184.3331235). 浙大 赵洲团队 [[code](https://github.com/ikuinen/CMIN_moment_retrieval)]
- [WACV'19] [MAC: Mining Activity Concepts for Language-based Temporal Localization](https://ieeexplore.ieee.org/abstract/document/8658811). 南加大 [[code](https://github.com/runzhouge/MAC)]

**Proposal-free**
- [AAAI'19] [Multilevel Language and Vision Integration for Text-to-Clip Retrieval](https://ojs.aaai.org/index.php/AAAI/article/view/4938). BU Huijuan Xu [[code](https://github.com/VisionLearningGroup/Text-to-Clip_Retrieval)]
- [AAAI'19] [To Find Where You Talk: Temporal Sentence Localization in Video with Attention Based Location Regression](https://ojs.aaai.org/index.php/AAAI/article/view/4950). 清华 朱文武团队 [[code](https://github.com/yytzsy/ABLR_code)]
- [EMNLP'19] [DEBUG: A Dense Bottom-Up Grounding Approach for Natural Language Video Localization](https://aclanthology.org/D19-1518/). 浙大 肖俊团队

**RL-based**
- [AAAI'19] [Read, Watch, and Move: Reinforcement Learning for Temporally Grounding Natural Language Descriptions in Videos](https://ojs.aaai.org/index.php/AAAI/article/view/4854). 百度
- [CVPR'19] [Language-Driven Temporal Activity Localization: A Semantic Matching Reinforcement Learning Model](https://openaccess.thecvf.com/content_CVPR_2019/html/Wang_Language-Driven_Temporal_Activity_Localization_A_Semantic_Matching_Reinforcement_Learning_Model_CVPR_2019_paper.html). 中科院 王亮团队
### <h3 id="weakly-supervised-2019">Weakly Supervised</h3>
**MIL-based**
- [CVPR'19] [Weakly Supervised Video Moment Retrieval From Text Queries](https://openaccess.thecvf.com/content_CVPR_2019/html/Mithun_Weakly_Supervised_Video_Moment_Retrieval_From_Text_Queries_CVPR_2019_paper.html). UCR Amit K. Roy-Chowdhury团队 [[code](https://github.com/niluthpol/weak_supervised_video_moment)]
    - 正式提出weakly supervised temporal sentence grounding任务。
- [EMNLP'19] [WSLLN:Weakly Supervised Natural Language Localization Networks](https://aclanthology.org/D19-1157/). Salesforce

## 2020
### <h3 id="fully-supervised-2020">Fully Supervised</h3>
**Proposal-based**
- [AAAI'20] [Learning 2D Temporal Adjacent Networks for Moment Localization with Natural Language](https://ojs.aaai.org/index.php/AAAI/article/view/6984). UR 罗杰波团队 [[code](https://github.com/microsoft/2D-TAN)]
	- 首次提出2D map的方法，后面proposal-based的论文大多都是基于这个方法。

**Proposal-free**
- [ACL'20] [Span-based Localizing Network for Natural Language Video Localization](https://aclanthology.org/2020.acl-main.585/). NTU 孙爱欣团队 [[code](https://github.com/26hzhang/VSLNet)]

### <h3 id="weakly-supervised-2020">Weakly Supervised</h3>
**Reconstruction-based**
- [AAAI'20] [Weakly-Supervised Video Moment Retrieval via Semantic Completion Network](https://ojs.aaai.org/index.php/AAAI/article/view/6820). 浙大 赵洲团队 [[code](https://github.com/ikuinen/semantic_completion_network)]
    - 首次在WTSG任务中使用掩码重建的方法。

## 2021
### <h3 id="fully-supervised-2021">Fully Supervised</h3>
**Proposal-based**
- [SIGIR'21] [Deconfounded Video Moment Retrieval with Causal Intervention](https://dl.acm.org/doi/abs/10.1145/3404835.3462823). NUS Tat-Seng Chua 团队 [[code](https://github.com/Xun-Yang/Causal_Video_Moment_Retrieval)]
	- 将因果推理引入TSG，消除视频中的位置信息带来的偏差
- [CVPR'21] [Interventional Video Grounding with Dual Contrastive Learning](https://openaccess.thecvf.com/content/CVPR2021/html/Nan_Interventional_Video_Grounding_With_Dual_Contrastive_Learning_CVPR_2021_paper.html). 北邮 南国顺
	- Contrastive learning + causal intervention
- [CVPR'21] [Multi-Modal Relational Graph for Cross-Modal Video Moment Retrieval](https://openaccess.thecvf.com/content/CVPR2021/html/Zeng_Multi-Modal_Relational_Graph_for_Cross-Modal_Video_Moment_Retrieval_CVPR_2021_paper.html). 湖南大学 曹达团队
- [ICCV'21] [Fast Video Moment Retrieval](https://openaccess.thecvf.com/content/ICCV2021/html/Gao_Fast_Video_Moment_Retrieval_ICCV_2021_paper.html). 中科院 徐常胜团队


**Proposal-free**
- [TPAMI'21] [Natural Language Video Localization: A Revisit in Span-Based Question Answering Framework](https://ieeexplore.ieee.org/abstract/document/9361191). NTU 孙爱欣团队
	- VSLNet (ACL'20)的扩展版
- [TMM'21] [Frame-Wise Cross-Modal Matching for Video Moment Retrieval](https://ieeexplore.ieee.org/abstract/document/9374685/). 齐鲁工业大学 程志勇团队 [[code](https://github.com/tanghaoyu258/ACRM-for-moment-retrieval)]

**DETR-based**
- [NeurIPS'21] [QVHighlights: Detecting Moments and Highlights in Videos via Natural Language Queries](https://proceedings.neurips.cc/paper/2021/hash/62e0973455fd26eb03e91d5741a4a3bb-Abstract.html). UNC 雷杰 [[code](https://github.com/jayleicn/moment_detr)]
    - 将MR和HD任务联合，首次将DETR引入VMR领域。

### <h3 id="zero-shot-2021">Zero-Shot</h3>
首次提出无监督任务。
- [ICCV'21] [Zero-shot Natural Language Video Localization](https://openaccess.thecvf.com/content/ICCV2021/html/Nam_Zero-Shot_Natural_Language_Video_Localization_ICCV_2021_paper.html). 首尔大学 Jonghyun Choi团队 [[code](https://github.com/gistvision/PSVL)]
- [TCSVT'21] [Learning Video Moment Retrieval Without a Single Annotated Video](https://ieeexplore.ieee.org/abstract/document/9415694). 中科院 徐常胜团队

## 2022
### <h3 id="fully-supervised-2022">Fully Supervised</h3>
**Proposal-based**
- [SIGIR'22] [You Need to Read Again: Multi-granularity Perception Network for Moment Retrieval in Videos](https://dl.acm.org/doi/abs/10.1145/3477495.3532083). 上交 周曦团队 [[code](https://github.com/Huntersxsx/MGPN)]
- [TCSVT'22] [Efficient Video Grounding With Which-Where Reading Comprehension](https://ieeexplore.ieee.org/abstract/document/9771472/). 上交 周曦团队

**Proposal-free**
- [TIP'22] [HiSA: Hierarchically Semantic Associating for Video Temporal Grounding](https://ieeexplore.ieee.org/abstract/document/9846867/). 西电 邓成团队 [[code](https://github.com/zhexu1997/HiSA)]

**DETR-based**
- [CVPR'22] [UMT: Unified Multi-modal Transformers for Joint Video Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2022/html/Liu_UMT_Unified_Multi-Modal_Transformers_for_Joint_Video_Moment_Retrieval_and_CVPR_2022_paper.html). 腾讯ARC lab [[code](https://github.com/TencentARC/UMT)]

### <h3 id="weakly-supervised-2022">Weakly Supervised</h3>
**Reconstruction-based**
- [AAAI'22] [Weakly Supervised Video Moment Localization with Contrastive Negative Sample Mining](https://ojs.aaai.org/index.php/AAAI/article/view/20263). 北大 刘洋团队 [[code](https://github.com/minghangz/cnm)]
- [CVPR'22] [Weakly Supervised Temporal Sentence Grounding with Gaussian-based Contrastive Proposal Learning](https://openaccess.thecvf.com/content/CVPR2022/html/Zheng_Weakly_Supervised_Temporal_Sentence_Grounding_With_Gaussian-Based_Contrastive_Proposal_Learning_CVPR_2022_paper.html). 北大 刘洋团队 [[code](https://github.com/minghangz/cpl)]
    - 挖掘负样本信息，以更好地区分同一视频中极易混淆的场景。
    - 后续的弱监督方法都是以CPL为baseline做的了。

### <h3 id="point-supervised/glance-2022">Point-supervised/Glance</h3>
首次提出单帧监督任务。
- [TMM'22] [Point-Supervised Video Temporal Grounding](https://ieeexplore.ieee.org/abstract/document/9882521). 西电 邓成团队
- [SIGIR'22] [Video Moment Retrieval from Text Queries via Single Frame Annotation](https://dl.acm.org/doi/abs/10.1145/3477495.3532078). 复旦 姜育刚团队 [[code](https://github.com/r-cui/ViGA)]

## 2023
### <h3 id="fully-supervised-2023">Fully Supervised</h3>
**Proposal-based**
- [AAAI'23] [Phrase-Level Temporal Relationship Mining for Temporal Sentence Localization](https://ojs.aaai.org/index.php/AAAI/article/view/25478). 北大 刘洋团队 [[code](https://github.com/minghangz/TRM)]
- [ICCV'23] [G2L: Semantically Aligned and Uniform Video Grounding via Geodesic and Game Theory](https://openaccess.thecvf.com/content/ICCV2023/html/Li_G2L_Semantically_Aligned_and_Uniform_Video_Grounding_via_Geodesic_and_ICCV_2023_paper.html). 北大 邹月娴团队

**Proposal-free**

**DETR-based**
- [ACL'23] [MS-DETR: Natural Language Video Localization with Sampling Moment-Moment Interaction](https://aclanthology.org/2023.acl-long.77/). NTU 孙爱欣团队 [[code](https://github.com/K-Nick/MS-DETR)]
- [CVPR'23] [Query-Dependent Video Representation for Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Moon_Query-Dependent_Video_Representation_for_Moment_Retrieval_and_Highlight_Detection_CVPR_2023_paper.html). 成均馆大学 Jae-Pil Heo团队 [[code](https://github.com/wjun0830/QD-DETR)]
- [ICCV'23] [Knowing Where to Focus: Event-aware Transformer for Video Grounding](https://openaccess.thecvf.com/content/ICCV2023/html/Jang_Knowing_Where_to_Focus_Event-aware_Transformer_for_Video_Grounding_ICCV_2023_paper.html). 延世大学 Kwanghoon Sohn团队 [[code](https://github.com/jinhyunj/EaTR)]
- [NeurIPS'23] [MomentDiff: Generative Video Moment Retrieval from Random to Real](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d01bda31bbcd780774ff15b534e03c40-Abstract-Conference.html). 中科大 谢洪涛团队 [[code](https://github.com/IMCCretrieval/MomentDiff)]
    - 利用diffusion的思想去噪生成预测时刻

**Bias**
- [AAAI'23] [Curriculum Multi-Negative Augmentation for Debiased Video Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/25204). 清华 朱文武团队
### <h3 id="weakly-supervised-2023">Weakly Supervised</h3>
**Reconstruction-based**
- [CVPR'23] [Weakly Supervised Temporal Sentence Grounding with Uncertainty-Guided Self-training](https://openaccess.thecvf.com/content/CVPR2023/html/Huang_Weakly_Supervised_Temporal_Sentence_Grounding_With_Uncertainty-Guided_Self-Training_CVPR_2023_paper.html). 东京大学 Yoichi Sato团队
- [CVPR'23] [Iterative Proposal Refinement for Weakly-Supervised Video Grounding](https://openaccess.thecvf.com/content/CVPR2023/html/Cao_Iterative_Proposal_Refinement_for_Weakly-Supervised_Video_Grounding_CVPR_2023_paper.html). 北大 邹月娴团队
- [ICCV'23] [SCANet: Scene Complexity Aware Network for Weakly-Supervised Video Moment Retrieval](https://openaccess.thecvf.com/content/ICCV2023/html/Yoon_SCANet_Scene_Complexity_Aware_Network_for_Weakly-Supervised_Video_Moment_Retrieval_ICCV_2023_paper.html). 韩国科学技术院 Chang D. Yoo团队
### <h3 id="point-supervised/glance-2023">Point-supervised/Glance</h3>
- [ICCV'23] [D3G: Exploring Gaussian Prior for Temporal Sentence Grounding with Glance Annotation](https://openaccess.thecvf.com/content/ICCV2023/html/Li_D3G_Exploring_Gaussian_Prior_for_Temporal_Sentence_Grounding_with_Glance_ICCV_2023_paper.html). 腾讯优图 [[code](https://github.com/solicucu/D3G)]
### <h3 id="zero-shot-2023">Zero-Shot</h3>
- [ACL'23] [Generating Structured Pseudo Labels for Noise-resistant Zero-shot Video Sentence Localization](https://aclanthology.org/2023.acl-long.794/). 北大 刘洋团队 [[code](https://github.com/minghangz/SPL)]

## 2024
### <h3 id="fully-supervised-2024">Fully Supervised</h3>
**Proposal-based**
- [ACM MM'24] [Maskable Retentive Network for Video Moment Retrieval](https://openreview.net/forum?id=pIHHAUa500). 合工大 汪萌团队 [[code](https://github.com/xian-sh/MRNet)]
- [AAAI'24] [Exploiting Auxiliary Caption for Video Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/29812). 北大 邹月娴团队

**Proposal-free**

**DETR-based**
- [AAAI'24] [Towards Balanced Alignment: Modal-Enhanced Semantic Modeling for Video Moment Retrieval](https://arxiv.org/abs/2312.12155). 中科大 谢洪涛团队 [[code](https://github.com/lntzm/MESM)]
    - 针对模态不平衡问题
- [AAAI'24] [TR-DETR: Task-Reciprocal Transformer for Joint Moment Retrieval and Highlight Detection](https://ojs.aaai.org/index.php/AAAI/article/view/28304). 华中师范 谢伟团队 [[code](https://github.com/mingyao1120/TR-DETR)]
- [CVPR'24] [Task-Driven Exploration: Decoupling and Inter-Task Feedback for Joint Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Task-Driven_Exploration_Decoupling_and_Inter-Task_Feedback_for_Joint_Moment_Retrieval_CVPR_2024_paper.html). 西交 魏平团队 [[code](https://github.com/EdenGabriel/TaskWeave)]
- [CVPR'24] [Bridging the Gap: A Unified Video Comprehension Framework for Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Xiao_Bridging_the_Gap_A_Unified_Video_Comprehension_Framework_for_Moment_CVPR_2024_paper.html). 清华 李秀团队 [[code](https://github.com/EasonXiao-888/UVCOM)]
- [ACM MM'24] [Prior Knowledge Integration via LLM Encoding and Pseudo Event Regulation for Video Moment Retrieval](https://arxiv.org/abs/2407.15051). 港浸大 魏骁勇团队 [[code](https://github.com/fletcherjiang/LLMEPET)]

**Bias**
- [AAAI'24] [Bias-Conflict Sample Synthesis and Adversarial Removal Debias Strategy for Temporal Sentence Grounding in Video](https://ojs.aaai.org/index.php/AAAI/article/view/28252). 哈工大 张维刚团队 [[code](https://github.com/qzhb/BSSARD)]
### <h3 id="weakly-supervised-2024">Weakly Supervised</h3>
**Reconstruction-based**
- [AAAI'24] [Gaussian Mixture Proposals with Pull-Push Learning Scheme to Capture Diverse Events for Weakly Supervised Temporal Video Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/28059). 首尔大学 Jin Young Choi团队 [[code](https://github.com/sunoh-kim/pps)]
- [AAAI'24] [Omnipotent Distillation with LLMs for Weakly-Supervised Natural Language Video Localization: When Divergence Meets Consistency](https://ojs.aaai.org/index.php/AAAI/article/view/27832). NTU Alex C. Kot团队
- [PR'24] [Triadic temporal-semantic alignment for weakly-supervised video moment retrieval](https://www.sciencedirect.com/science/article/pii/S0031320324005703). 山东大学 周风余团队
- [ACL'24] [Exploiting Intrinsic Multilateral Logical Rules for Weakly Supervised Natural Language Video Localization](https://aclanthology.org/2024.acl-long.247/). 西电 邓成团队

## 2025
### <h3 id="fully-supervised-2025">Fully Supervised</h3>
- [AAAI'25] [Diversifying Query: Region-Guided Transformer for Temporal Sentence Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/32766). [[code](https://github.com/TensorsSun/RGTR)]
- [ICCV'25] [KDA: Knowledge Diffusion Alignment with Enhanced Context  for Video Temporal Grounding](https://openaccess.thecvf.com/content/ICCV2025/html/Ran_KDA_Knowledge_Diffusion_Alignment_with_Enhanced_Context_for_Video_Temporal_ICCV_2025_paper.html).
- [ICCV'25] [Sim-DETR: Unlock DETR for temporal sentence grounding](https://openaccess.thecvf.com/content/ICCV2025/html/Tang_Sim-DETR_Unlock_DETR_for_Temporal_Sentence_Grounding_ICCV_2025_paper.html).
- [ICCV'25] [Vid-Group: Temporal Video Grounding Pretraining  from Unlabeled Videos in the Wild](https://openaccess.thecvf.com/content/ICCV2025/html/Bao_Vid-Group_Temporal_Video_Grounding_Pretraining_from_Unlabeled_Videos_in_the_ICCV_2025_paper.html).
- [MM'25] [Boosting Temporal Sentence Grounding via Causal Inference](https://dl.acm.org/doi/abs/10.1145/3746027.3755624). [[code](https://github.com/Tangkfan/CICR)]
- [MM'25] [Turing Patterns for Multimedia: Reaction-Diffusion Multi-Modal Fusion for Language-Guided Video Moment Retrieval](https://dl.acm.org/doi/abs/10.1145/3746027.3758179).
- [MM'25] [Audio Does Matter: Importance-Aware Multi-Granularity Fusion for Video Moment Retrieval](https://dl.acm.org/doi/abs/10.1145/3746027.3754982).
- [NeurIPS'25] [CausalVTG: Towards robust video temporal grounding via causal inference](https://openreview.net/forum?id=oeWgBOowL6).
- [NeurIPS'25] [SpikingVTG: A Spiking Detection Transformer for Video Temporal Grounding](https://openreview.net/forum?id=SkhF3cuyev).


### <h3 id="weakly-supervised-2025">Weakly Supervised</h3>
- [ICASSP'25] [FAWL: Weakly-supervised video corpus moment retrieval with frame-wise auxiliary alignment and weighted contrastive learning](https://ieeexplore.ieee.org/abstract/document/10887823). [[code](https://github.com/BUAAPY/FAWL)]
- [NeurIPS'25] [PC-Net: Weakly Supervised Compositional Moment Retrieval via Proposal-Centric Network](https://openreview.net/forum?id=kQAnOaayIo). [[code](https://github.com/mingyao1120/PC-Net)]

### <h3 id="point-supervised-2025">Point-Supervised/Glance</h3>
- [SIGIR'25] [Gaming for Boundary: Elastic Localization for Frame-Supervised Video Moment Retrieval](https://dl.acm.org/doi/abs/10.1145/3726302.3729984). 
