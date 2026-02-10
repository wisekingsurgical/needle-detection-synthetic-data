# needle-detection-synthetic-data

This repository provides the official implementation and dataset access for the paper:

**Finding the Sweet Spot: Systematic Analysis and Robotic Validation of Synthetic Data for Few-Shot Endoscopic Needle Detection**  
(*to appear in MICCAI 2026, under review*)

We investigate how the **scale and design of synthetic data** affect real-world performance in **few-shot endoscopic needle detection**, with systematic experiments and **robotic validation**.

---

## 🔍 Overview

Accurate detection of surgical needles in endoscopic images is critical for robotic minimally invasive surgery. However, training robust deep learning models is challenging due to the **limited availability and high annotation cost of real intraoperative data**.

Synthetic data has been widely adopted to mitigate data scarcity, yet **how much synthetic data to use—and how to design it—remains an open question**, especially in safety-critical medical applications.

This project addresses this gap by:

- Conducting a **systematic analysis** of synthetic data volume under fixed real-data budgets
- Revealing an **inverted U-shaped relationship** between synthetic data scale and real-world performance
- Proposing a **targeted synthetic data generation strategy** guided by real-data failure cases
- Validating findings not only offline but also on a **robotic experimental platform**

---

## ✨ Key Contributions

- **Systematic Evaluation**  
  A controlled study of synthetic data scaling effects in few-shot endoscopic needle detection.

- **Targeted Synthetic Data Design**  
  A failure-aware synthesis strategy focusing on challenging scenarios such as occlusion and extreme viewpoints.

- **Robotic Validation**  
  Experimental verification of detection stability and robustness within a robotic workflow.

- **Open Dataset & Code**  
  Public release of a synthetic endoscopic needle dataset and reproducible experimental configurations.

---

## 📂 Repository Structure

```text
synthetic-endoscopic-needle-detection/
├── README.md
├── LICENSE
├── CITATION.cff
├── docs/
│   ├── dataset_description.md
│   ├── synthetic_pipeline.md
│   ├── robot_validation.md
│   └── ethics_statement.md
├── data/
│   ├── README.md
│   └── download_links.md
├── annotations/
│   ├── format.md
│   └── examples/
├── code/
│   ├── training/
│   ├── evaluation/
│   └── configs/
└── examples/
    └── visualization.ipynb
