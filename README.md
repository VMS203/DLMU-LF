# DLMU-LF

A large-scale light field salient object detection benchmark dataset developed for multiple research fields. If you find that our data violates your rights, please contact us immediately, and we will deal with it in time.

### Abstract

Salient Object Detection (SOD) aims to simulate the human visual attention mechanism to automatically locate and segment the most visually attractive objects in complex scenes. However, existing light field SOD datasets suffer from limited data quality and insufficient category diversity, which hinders the development of light field SOD. Moreover, current methods still face challenges in fully exploiting the valuable depth cues and diverse focus features within focal stacks. To address these problems, we construct a large-scale benchmark dataset for light field SOD, named DLMU-LF. It contains 5,037 samples with comprehensive annotations and covers diverse object categories. 
Based on this dataset, we propose a novel framework, Reconstruction-guided Light Field Salient Object Detection Network (RLFSNet), which leverages focal stack reconstruction of all-in-focus images to assist salient object detection. Specifically, RLFSNet introduces an all-in-focus reconstruction branch to synthesize complete scene representations and alleviate the discreteness of focal stacks. In addition, we design a Hierarchical Selective Fusion (HSF) module and a Frequency Guided Feature Fusion (FGFF) module to model cross-slice dependencies and enhance cross-modal features. 
Extensive experiments demonstrate that RLFSNet achieves superior performance over state-of-the-art methods across multiple benchmark datasets, while maintaining stable performance and strong generalization in complex scenarios.

![Figure 1](figures/dataset_pic_fix.png)

_Fig. 1: Dataset quantitative feature distribution. (a) Salient object categories; (b) Scenario complexity; (c) Size distribution of salient objects; (d) Spatial distribution of salient objects; (e) Multi-object proportion._

### Dataset

[![License: CC BY-NC-ND 4.0](https://img.shields.io/badge/License-CC%20BY--NC--ND%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-nd/4.0/) Usage of our dataset is under the Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International Public License.

![Figure 2](figures/dataset_examplenew.png)

_Fig. 2: Representative examples from the proposed DLMU-LF dataset. The dataset contains diverse scenes with significant object scale variations and complex backgrounds. Each sample is provided with multiple types of annotations, offering rich supervision information and supporting comprehensive research on light field salient object detection._

**Download (full package):**

- [Baidu Netdisk](https://pan.baidu.com/s/1ySPZhBSDq390_YFMO6dKnQ?pwd=dlmu) (extraction code: `dlmu`)
- Google Drive: _Coming soon_

The full package contains all data types (original light field data, all-in-focus images, depth maps, 12-frame focal stacks, multi-view arrays, edge maps, and annotations) and is distributed across 5 sub-packages (3 for training and 2 for testing).

#### Dataset Statistics

| Item | Detail |
|:--|:--|
| Total samples | 5,037 (5,004 normal + 33 negative) |
| Categories | 11 primary categories, 145 subcategories |
| Camera | Lytro Illum |
| Resolution | 2450 × 1634 (high) / 256 × 256 (low) |
| Data partition | 5 packages (3 training / 2 testing); 3,025 train / 2,012 test |
| Per-sample contents | Original light field data, all-in-focus image, depth map, 12 focal stack images, multi-view image array, edge map, label map |
| Annotations | Scribbles, points, bounding boxes, instance masks |
| Decoding tools | Lytro Power Tools (LPT), Lytro Desktop |

### Contact

- **Corresponding author:** Pengjie Wang (pengjiewang@gmail.com)
- **Affiliation:** College of Computer Science and Engineering, Dalian Minzu University, Dalian 116600, China
- **Issue / Q&A:** Please use the [GitHub Issues](../../issues) of this repository.
