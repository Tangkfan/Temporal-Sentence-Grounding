# Temporal Sentence Grounding

List of Temporal Sentence Grounding papers.

The task is also usually referred to as:
- Temporal Sentence Grounding (TSG)
- Video Moment Retrieval (VMR)
- Temporal Activity Localization via Language Query (TALL)

# Content
- [1 Survey](#1-Survey)
- [2 Datasets](#2-Datasets)
- [3 Paper](#3-Paper)
    - [2017](#2017)-[2018](#2018)-[2019](#2019)
    - [2020](#2020)-[2021](#2021)-[2022](#2022)
    - [2023](#2023)-[2024](#2024)

# 1 Survey
- [TPAMI'23][Temporal Sentence Grounding in Videos: A Survey and Future Directions](https://ieeexplore.ieee.org/abstract/document/10075491). NTU 孙爱欣团队 
- [ACM Comput. Surv.'23] [A Survey on Video Moment Localization](https://dl.acm.org/doi/abs/10.1145/3556537). 哈工大 聂礼强团队

# 2 Datasets
- Charades-STA: [VGG](https://github.com/TencentARC/UMT), [C3D](https://rochester.app.box.com/s/swu6rlqcdlebvwml8dyescmi7ra0owc5), [I3D](https://app.box.com/s/h0sxa5klco6qve5ahnz50ly2nksmuedw/folder/138545516584), [CLIP+SF](https://mailustceducn-my.sharepoint.com/personal/liuzhihang_mail_ustc_edu_cn/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fliuzhihang%5Fmail%5Fustc%5Fedu%5Fcn%2FDocuments%2FOpenSource%2FMESM%2Fdata&ga=1)
- TACoS: [C3D](https://app.box.com/s/h0sxa5klco6qve5ahnz50ly2nksmuedw/folder/138544435150), [I3D](https://rochester.app.box.com/s/swu6rlqcdlebvwml8dyescmi7ra0owc5)
- ActivityNet Captions: [C3D](http://activity-net.org/challenges/2016/download.html)
- QVHighlights: [CLIP+SF](https://github.com/jayleicn/moment_detr)

# 3 Paper
## 2017
首次提出TSG任务。
### Fully Supervised
**Proposal-based**
- [ICCV'17] [TALL: Temporal Activity Localization via Language Query](https://openaccess.thecvf.com/content_iccv_2017/html/Gao_TALL_Temporal_Activity_ICCV_2017_paper.html). 南加大 高继扬 [[code](https://github.com/jiyanggao/TALL)]
- [ICCV'17] [Localizing Moments in Video with Natural Language](https://openaccess.thecvf.com/content_iccv_2017/html/Hendricks_Localizing_Moments_in_ICCV_2017_paper.html). 伯克利 Lisa Anne Hendricks [[code](https://github.com/LisaAnne/LocalizingMoments)]

## 2018
### Fully Supervised
**Proposal-based**

### Weakly Supervised
**Reconstruction-based**
- [NeurIPS'18] [Weakly Supervised Dense Event Captioning in Videos](https://proceedings.neurips.cc/paper/2018/hash/49af6c4e558a7569d80eee2e035e2bd7-Abstract.html). 清华 朱文武团队 [[code](https://github.com/ranjaykrishna/densevid_eval)]
    - 首次提出弱监督密集事件描述，在训练中涉及到了TSG问题

## 2019
### Fully Supervised
**Proposal-based**

### Weakly Supervised
**MIL-based**
- [CVPR'19] [Weakly Supervised Video Moment Retrieval From Text Queries](https://openaccess.thecvf.com/content_CVPR_2019/html/Mithun_Weakly_Supervised_Video_Moment_Retrieval_From_Text_Queries_CVPR_2019_paper.html). UCR Amit K. Roy-Chowdhury团队 [[code](https://github.com/niluthpol/weak_supervised_video_moment)]
    - 正式提出weakly supervised temporal sentence grounding任务。

## 2020 
### Fully Supervised
**Proposal-based**

**Proposal-free**

### Weakly Supervised
**Reconstruction-based**
- [AAAI'20] [Weakly-Supervised Video Moment Retrieval via Semantic Completion Network](https://ojs.aaai.org/index.php/AAAI/article/view/6820). 浙大 赵洲团队 [[code](https://github.com/ikuinen/semantic_completion_network)]
    - 首次在WTSG任务中使用掩码重建的方法。

## 2021
### Fully Supervised
**Proposal-based**

**Proposal-free**

**DETR-based**
- [NeurIPS'21] [QVHighlights: Detecting Moments and Highlights in Videos via Natural Language Queries](https://proceedings.neurips.cc/paper/2021/hash/62e0973455fd26eb03e91d5741a4a3bb-Abstract.html). UNC 雷杰 [[code](https://github.com/jayleicn/moment_detr)]
    - 将MR和HD任务联合，首次将DETR引入VMR领域。

### Zero-shot
首次提出无监督任务。
- [ICCV'21] [Zero-shot Natural Language Video Localization](https://openaccess.thecvf.com/content/ICCV2021/html/Nam_Zero-Shot_Natural_Language_Video_Localization_ICCV_2021_paper.html). 首尔大学 Jonghyun Choi团队 [[code](https://github.com/gistvision/PSVL)]
- [TCSVT'21] [Learning Video Moment Retrieval Without a Single Annotated Video](https://ieeexplore.ieee.org/abstract/document/9415694). 中科院 徐常胜团队

## 2022
### Fully Supervised
**Proposal-based**
- [SIGIR'22] [You Need to Read Again: Multi-granularity Perception Network for Moment Retrieval in Videos](https://dl.acm.org/doi/abs/10.1145/3477495.3532083). 上交 周曦团队 [[code](https://github.com/Huntersxsx/MGPN)]

**Proposal-free**

**DETR-based**

### Weakly Supervised
**Reconstruction-based**
- [AAAI'22] [Weakly Supervised Video Moment Localization with Contrastive Negative Sample Mining](https://ojs.aaai.org/index.php/AAAI/article/view/20263). 北大 刘洋团队 [[code](https://github.com/minghangz/cnm)]
- [CVPR'22] [Weakly Supervised Temporal Sentence Grounding with Gaussian-based Contrastive Proposal Learning](https://openaccess.thecvf.com/content/CVPR2022/html/Zheng_Weakly_Supervised_Temporal_Sentence_Grounding_With_Gaussian-Based_Contrastive_Proposal_Learning_CVPR_2022_paper.html). 北大 刘洋团队 [[code](https://github.com/minghangz/cpl)]
    - 挖掘负样本信息，以更好地区分同一视频中极易混淆的场景。
    - 后续的弱监督方法都是以CPL为baseline做的了。

### Point-supervised/Glance
首次提出单帧监督任务。
- [TMM'22] [Point-Supervised Video Temporal Grounding](https://ieeexplore.ieee.org/abstract/document/9882521). 西电 邓成团队
- [SIGIR'22] [Video Moment Retrieval from Text Queries via Single Frame Annotation](https://dl.acm.org/doi/abs/10.1145/3477495.3532078). 复旦 姜育刚团队 [[code](https://github.com/r-cui/ViGA)]

## 2023
### Fully Supervised
**Proposal-based**
- [AAAI'23] [Phrase-Level Temporal Relationship Mining for Temporal Sentence Localization](https://ojs.aaai.org/index.php/AAAI/article/view/25478). 北大 刘洋团队 [[code](https://github.com/minghangz/TRM)]

**Proposal-free**

**DETR-based**
- [ACL'23] [MS-DETR: Natural Language Video Localization with Sampling Moment-Moment Interaction](https://aclanthology.org/2023.acl-long.77/). NTU 孙爱欣团队 [[code](https://github.com/K-Nick/MS-DETR)]
- [CVPR'23] [Query-Dependent Video Representation for Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Moon_Query-Dependent_Video_Representation_for_Moment_Retrieval_and_Highlight_Detection_CVPR_2023_paper.html). 成均馆大学 Jae-Pil Heo团队 [[code](https://github.com/wjun0830/QD-DETR)]
- [ICCV'23] [Knowing Where to Focus: Event-aware Transformer for Video Grounding](https://openaccess.thecvf.com/content/ICCV2023/html/Jang_Knowing_Where_to_Focus_Event-aware_Transformer_for_Video_Grounding_ICCV_2023_paper.html). 延世大学 Kwanghoon Sohn团队 [[code](https://github.com/jinhyunj/EaTR)]
- [NeurIPS'23] [MomentDiff: Generative Video Moment Retrieval from Random to Real](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d01bda31bbcd780774ff15b534e03c40-Abstract-Conference.html). 中科大 谢洪涛团队 [[code](https://github.com/IMCCretrieval/MomentDiff)]
    - 利用diffusion的思想去噪生成预测时刻
 
### Weakly Supervised
**Reconstruction-based**
- [CVPR'23] [Weakly Supervised Temporal Sentence Grounding with Uncertainty-Guided Self-training](https://openaccess.thecvf.com/content/CVPR2023/html/Huang_Weakly_Supervised_Temporal_Sentence_Grounding_With_Uncertainty-Guided_Self-Training_CVPR_2023_paper.html). 东京大学 Yoichi Sato团队
- [CVPR'23] [Iterative Proposal Refinement for Weakly-Supervised Video Grounding](https://openaccess.thecvf.com/content/CVPR2023/html/Cao_Iterative_Proposal_Refinement_for_Weakly-Supervised_Video_Grounding_CVPR_2023_paper.html). 北大 邹月娴团队

### Zero-shot
- [ACL'23] [Generating Structured Pseudo Labels for Noise-resistant Zero-shot Video Sentence Localization](https://aclanthology.org/2023.acl-long.794/). 北大 刘洋团队 [[code](https://github.com/minghangz/SPL)]

## 2024
### Fully Supervised
**Proposal-based**

**Proposal-free**

**DETR-based**
- [AAAI'24] [Towards Balanced Alignment: Modal-Enhanced Semantic Modeling for Video Moment Retrieval](https://arxiv.org/abs/2312.12155). 中科大 谢洪涛团队 [[code](https://github.com/lntzm/MESM)]
    - 针对模态不平衡问题
- [AAAI'24] [TR-DETR: Task-Reciprocal Transformer for Joint Moment Retrieval and Highlight Detection](https://ojs.aaai.org/index.php/AAAI/article/view/28304). 华中师范 谢伟团队 [[code](https://github.com/mingyao1120/TR-DETR)]
- [CVPR'24] [Task-Driven Exploration: Decoupling and Inter-Task Feedback for Joint Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Task-Driven_Exploration_Decoupling_and_Inter-Task_Feedback_for_Joint_Moment_Retrieval_CVPR_2024_paper.html). 西交 魏平团队 [[code](https://github.com/EdenGabriel/TaskWeave)]
- [CVPR'24] [Bridging the Gap: A Unified Video Comprehension Framework for Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2024/html/Xiao_Bridging_the_Gap_A_Unified_Video_Comprehension_Framework_for_Moment_CVPR_2024_paper.html). 清华 李秀团队 [[code](https://github.com/EasonXiao-888/UVCOM)]

**Bias**
- [AAAI'24] [Bias-Conflict Sample Synthesis and Adversarial Removal Debias Strategy for Temporal Sentence Grounding in Video](https://ojs.aaai.org/index.php/AAAI/article/view/28252). 哈工大 张维刚团队 [[code](https://github.com/qzhb/BSSARD)]

### Weakly Supervised
**Reconstruction-based**
- [AAAI'24] [Gaussian Mixture Proposals with Pull-Push Learning Scheme to Capture Diverse Events for Weakly Supervised Temporal Video Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/28059). 首尔大学 Jin Young Choi团队 [[code](https://github.com/sunoh-kim/pps)]
- [PR'24] [Triadic temporal-semantic alignment for weakly-supervised video moment retrieval](https://www.sciencedirect.com/science/article/pii/S0031320324005703). 山东大学 周风余团队
