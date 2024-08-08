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
## 2018
## 2019
## 2020 
## 2021
**DETR-based**
- [NeurIPS'21] [QVHighlights: Detecting Moments and Highlights in Videos via Natural Language Queries](https://proceedings.neurips.cc/paper/2021/hash/62e0973455fd26eb03e91d5741a4a3bb-Abstract.html). UNC 雷杰 [[code](https://github.com/jayleicn/moment_detr)]
    - 将MR和HD任务联合，首次将DETR引入VMR领域。

## 2022
## 2023
### Fully Supervised
**DETR-based**
- [ACL'23] [MS-DETR: Natural Language Video Localization with Sampling Moment-Moment Interaction](https://aclanthology.org/2023.acl-long.77/). NTU 孙爱欣团队 [[code](https://github.com/K-Nick/MS-DETR)]
- [CVPR'23] [Query-Dependent Video Representation for Moment Retrieval and Highlight Detection](https://openaccess.thecvf.com/content/CVPR2023/html/Moon_Query-Dependent_Video_Representation_for_Moment_Retrieval_and_Highlight_Detection_CVPR_2023_paper.html). 成均馆大学 Jae-Pil Heo团队 [[code](https://github.com/wjun0830/QD-DETR)]
- [ICCV'23] [Knowing Where to Focus: Event-aware Transformer for Video Grounding](https://openaccess.thecvf.com/content/ICCV2023/html/Jang_Knowing_Where_to_Focus_Event-aware_Transformer_for_Video_Grounding_ICCV_2023_paper.html). 延世大学 Kwanghoon Sohn团队 [[code](https://github.com/jinhyunj/EaTR)]
- [NeurIPS'23] [MomentDiff: Generative Video Moment Retrieval from Random to Real](https://proceedings.neurips.cc/paper_files/paper/2023/hash/d01bda31bbcd780774ff15b534e03c40-Abstract-Conference.html). 中科大 谢洪涛团队 [[code](https://github.com/IMCCretrieval/MomentDiff)]
    - 利用diffusion的思想去噪生成预测时刻

## 2024
### Fully Supervised
**DETR-based**
- [AAAI'24] [Towards Balanced Alignment: Modal-Enhanced Semantic Modeling for Video Moment Retrieval](https://arxiv.org/abs/2312.12155). 中科大 谢洪涛团队 [[code](https://github.com/lntzm/MESM)]
    - 针对模态不平衡问题
- [AAAI'24] [TR-DETR: Task-Reciprocal Transformer for Joint Moment Retrieval and Highlight Detection](https://ojs.aaai.org/index.php/AAAI/article/view/28304). 华中师范 谢伟团队 [[code](https://github.com/mingyao1120/TR-DETR)]

**Bias**
- [AAAI'24] [Bias-Conflict Sample Synthesis and Adversarial Removal Debias Strategy for Temporal Sentence Grounding in Video](https://ojs.aaai.org/index.php/AAAI/article/view/28252). 哈工大 张维刚团队 [[code](https://github.com/qzhb/BSSARD)]

### Weakly Supervised
- [AAAI'24] [Gaussian Mixture Proposals with Pull-Push Learning Scheme to Capture Diverse Events for Weakly Supervised Temporal Video Grounding](https://ojs.aaai.org/index.php/AAAI/article/view/28059). 首尔大学 Jin Young Choi团队 [[code](https://github.com/sunoh-kim/pps)]
- [PR'24] [Triadic temporal-semantic alignment for weakly-supervised video moment retrieval](https://www.sciencedirect.com/science/article/pii/S0031320324005703). 山东大学 周风余团队
