# Crosswalk Segmentation with DeepLabv3 + ConvNeXt

This repository contains the implementation of our research on **crosswalk segmentation** for autonomous driving. The study evaluates the effectiveness of **DeepLabv3** with two different backbones: **ResNet50** (baseline) and **ConvNeXt-Tiny** (proposed).  

---

## 📑 Abstract
Crosswalk segmentation plays a critical role in autonomous driving by ensuring pedestrian safety and compliance with traffic regulations. This study investigates the performance of DeepLabv3 with ResNet50 and ConvNeXt-Tiny backbones on the **FPVCrosswalk2025** dataset (3,300 images across sunny, cloudy, rainy, nighttime, and neutral conditions). Results show that ConvNeXt-Tiny consistently outperformed ResNet50, with IoU gains of 0.3–0.7% on average and up to 2.5% in adverse weather and low-light conditions. These findings highlight ConvNeXt’s favorable trade-off between accuracy, robustness, and efficiency, making it a practical backbone for real-time, safety-critical driving systems.  

---

## 📂 Dataset

- **FPVCrosswalk2025**: 3,000 synthetic + 300 real-world images (total 3,300), each paired with a binary segmentation mask.  
- Environmental conditions: sunny, cloudy, rainy, nighttime, neutral.  
- Dataset paper: *“FPVCrosswalk2025: A dataset for first-person view crosswalk segmentation in adverse weather and lighting conditions”*, DOI: **10.1016/j.dib.2025.111755**.  
- Dataset repository: Mendeley Data, version 1 — [FPVCrosswalk2025 on Mendeley Data](https://data.mendeley.com/datasets/mcr2jwk5bp/1)  
- License: **CC BY 4.0**  


---

## ⚙️ Installation
```bash
git clone https://github.com/username/crosswalk-segmentation.git
cd crosswalk-segmentation
pip install -r requirements.txt
```
📊 Results
Backbone	mIoU	Dice	Precision	Recall
ResNet50	93.17	96.47	96.30	96.63
ConvNeXt-Tiny	93.47	96.62	97.02	96.23

This project is released under the MIT License.
