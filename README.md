# [IndoorMS: A Multispectral Dataset for Semantic Segmentation in Indoor Scene Understanding](https://doi.org/10.1109/JSEN.2025.3559348)
This is the official repository for "IndoorMS: A Multispectral Dataset for Semantic Segmentation in Indoor Scene Understanding". {[IEEE](https://doi.org/10.1109/JSEN.2025.3559348)}

## Abstract

Indoor scene understanding is a critical task in computer vision, traditionally relying on RGB data for deep learning-based semantic segmentation to achieve pixel-level understanding. However, indoor environments provide valuable information beyond the visible light spectrum, which has been largely overlooked in existing research. To address this gap, we introduce IndoorMS, a comprehensive multispectral dataset specifically designed for the semantic segmentation of indoor scenes. The dataset comprises images captured using a multispectral sensor in 17 buildings across diverse indoor settings, including meeting rooms, halls, lounges, offices, corridors, and classrooms. With 19 finely annotated semantic categories, IndoorMS enables robust evaluation of indoor scene segmentation. Benchmark experiments are performed using several leading semantic segmentation frameworks, followed by a thorough analysis of their performance. The results indicate that the optimal model combination, namely ConvNeXt-s with UperNet, achieved an mF1 score of 82.38 and an mIoU score of 72.90. Despite these promising results, IndoorMS’s challenges on segmentation networks remain, such as class distribution imbalance and domain gaps between RGB and multispectral data. This work marks the first effort to support multispectral indoor scene understanding with a dedicated dataset, offering new opportunities for research in this domain. Potential avenues for future research are presented. The project page for the IndoorMS dataset is available at https://zhuqinfeng1999.github.io/IndoorMS/.

## Overview

- **Dataset Name:** IndoorMS
- **Purpose:** To facilitate semantic segmentation of indoor scenes using multispectral data.
- **Content:** Multispectral images from 17 buildings, covering various indoor environments such as meeting rooms, halls, lounges, offices, corridors, and classrooms.
- **Annotations:** 19 semantic categories with fine annotations.
- **Format:** Structured based on the mmsegmentation framework.

## Download

The IndoorMS dataset, including multispectral images, annotations, pseudo-color images, and reference cell phone images, is available for download:

- Full Dataset (Google Drive)
- Pseudo-color and Reference Images (Google Drive)

## Dataset Structure

The IndoorMS dataset is organized as follows:

```bash
IndoorMS/
├── ann_dir/
│   ├── train/
│   │   └── <image_name>.png
│   ├── val/
│   │   └── <image_name>.png
│   └── test/
│       └── <image_name>.png
└── img_dir/
    ├── train/
    │   └── <image_name>.tif
    ├── val/
    │   └── <image_name>.tif
    └── test/
        └── <image_name>.tif
```

- **img_dir:** Contains the multispectral images in TIFF format.
- **ann_dir:** Contains the annotation masks in PNG format.
- Each image in `img_dir` has a corresponding annotation mask in `ann_dir` with the same filename but different extension.
- We found that image number 29 had an error and has been removed from the provided dataset.

## Citation

If you find this work useful in your research, please consider citing:

```bibtex
@ARTICLE{10965893,
  author={Zhu, Qinfeng and Xiao, Jingjing and Fan, Lei},
  journal={IEEE Sensors Journal}, 
  title={IndoorMS: A Multispectral Dataset for Semantic Segmentation in Indoor Scene Understanding}, 
  year={2025},
  volume={},
  number={},
  pages={1-1},
  keywords={Sensors;Semantic segmentation;Lighting;Data collection;Indoor environment;Annotations;Semantics;Intelligent sensors;Buildings;Training;Multispectral;Image;Dataset;Semantic Segmentation;Indoor;Scene Understanding},
  doi={10.1109/JSEN.2025.3559348}}
```

## Project Page

https://zhuqinfeng1999.github.io/IndoorMS/

---

*This repository is maintained by zhuqinfeng1999. For any questions or issues, please open an issue on GitHub.*
