# SiamTIH
The official PyTorch implementation of our paper, coming soon.

### :bookmark:Brief Introduction
RGB-T Siamese trackers have drawn continuous interest in recent years due to their proper trade-off between accuracy and speed. However, they are sensitive to the background distractors in some challenging cases, thereby inducing unreliable response positions. To overcome such drawbacks, we advance a new RGB-T Siamese tracker, named SiamTIH, which will advance the RGB-T Siamese trackers’ discriminability against distractors by exploiting target-related information and reliable global pixel relationships within multi-modal data.  Specifically, we propose a target-related feature enhancement module (TFE) to highlight such areas in the detection branch that are similar to the templates and suppress those background distractor regions that are significantly different from the templates but are greatly informative. Then, we propose an intra- and mutual-modal attention based multi-modal feature fusion module (IMA-MF) to capture the reliable global pixel relationships within multi-modal data. Especially, the intra-modal attention is used to capture the global pixel relationships within each single modality data, and the mutual-modal attention is utilized to enhance the feature representation of the current modality by overall pixel relationships as well as modality-specific relationships. Finally, we propose a hard-focused online classifier (HFOC) that combines an offline classifier and an online classifier to further improve the robustness of our tracker. Besides, the proposed framework is further extended to a Transformer based tracker to verify its generality. Extensive experiments on three RGB-T benchmarks demonstrate that our new RGB-T tracker outperforms the existing ones and maintains real-time performance, exceeding on average 30 frames per second (FPS).

### :bookmark:Strong Performance

|             Variant             |     GTOT (PR / SR )     |     RGBT234 (PR / SR )  |  LasHeR (PR / NPR/ SR ) |
|:-------------------------------:|:-----------------------:|:-----------------------:|:-----------------------:|
|          SiamTIH (Ours)         |       91.7 / 75.7       |         85.1 / 60.4     |     61.6 / 56.0 / 46.7  |
|          TransTIH (Ours)        |       93.5 / 77.0       |         89.4 / 66.4     |     72.0 / 67.7 / 57.2  |
|          TBSI  (CVPR2023)       |         - / -           |         87.1 / 63.7     |     69.2 / 65.7 / 55.6  |

# Raw results
[Download here](https://drive.google.com/file/d/1qviQkbEIBh8s-xt75YBSl3YfqelhbV5U/view?usp=sharing)

# To do
The code will be available after acceptance.

# Acknowledgment
This repo is based on SAOT, ViPT and OSTrack, helps us to quickly implement our ideas.

- [SAOT](https://github.com/ZikunZhou/SAOT) [[related paper](https://https://arxiv.org/abs/2108.03637)]
- [OSTrack](https://github.com/botaoye/OSTrack) [[related paper](https://arxiv.org/abs/2203.11991)]
- [ViPT](https://github.com/ZikunZhou/SAOT)[[related paper](https://openaccess.thecvf.com/content/CVPR2023/html/Zhu_Visual_Prompt_Multi-Modal_Tracking_CVPR_2023_paper.html)]


