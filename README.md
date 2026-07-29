# 🧠 Intracranial Aneurysm Detection Using Deep Learning

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![EfficientNet](https://img.shields.io/badge/EfficientNet-B0-green)
![Medical Imaging](https://img.shields.io/badge/DICOM-Medical%20Imaging-orange)
![Computer Vision](https://img.shields.io/badge/Computer-Vision-blueviolet)
![Transfer Learning](https://img.shields.io/badge/Transfer-Learning-success)
![Healthcare](https://img.shields.io/badge/Domain-Healthcare-red)

---

# ⭐ Project Highlights

- Developed an end-to-end deep learning pipeline for intracranial aneurysm detection from DICOM CT angiography images.
- Performed DICOM preprocessing, normalization, exploratory medical image analysis, and visualization.
- Generated localization-aware **2.5D image inputs** using neighboring CT slices and expert aneurysm annotations.
- Fine-tuned an **EfficientNet-B0** transfer learning model for binary aneurysm classification.
- Evaluated model performance using **ROC-AUC, Precision, Recall, F1-score, Confusion Matrix, and Threshold Analysis.**
- Built clinical visualization utilities to compare predictions with radiologist annotations.
- Demonstrated an AI-assisted workflow for medical image screening and computer-aided diagnosis.

---

# 📂 Repository Structure

```
Intracranial-Aneurysm-Detection/

│── rsna-intracranial-aneurysm-detection-portfolio.ipynb
│── README.md
│── requirements.txt
│
├── images/
│ └── README.md
│
└── docs/
└── README.md
```

---

# 📖 Project Overview

Intracranial aneurysms are weakened blood vessel walls inside the brain that may rupture and cause life-threatening hemorrhagic strokes. Early detection from CT Angiography (CTA) images is challenging because aneurysms are often very small and can resemble surrounding vessels.

This project develops an end-to-end deep learning workflow for automated aneurysm detection using the RSNA Intracranial Aneurysm Detection Challenge dataset. The pipeline combines DICOM preprocessing, localization-aware data preparation, transfer learning, and comprehensive evaluation to demonstrate how artificial intelligence can support radiologists during medical image interpretation.

---

# 🏥 Clinical Background

Brain aneurysms affect millions of people worldwide, yet many remain undiagnosed until rupture.

Challenges include:

- Extremely small lesion sizes
- Large volumetric CT studies
- High similarity between aneurysms and normal blood vessels
- Significant class imbalance

Artificial Intelligence can assist radiologists by:

- Prioritizing suspicious examinations
- Reducing missed aneurysms
- Improving screening efficiency
- Supporting clinical decision making

---

# 📊 Dataset

**Competition**

RSNA Intracranial Aneurysm Detection Challenge

Dataset consists of:

- CT Angiography (CTA) scans
- DICOM medical images
- Expert radiologist annotations
- Localization coordinates
- Binary aneurysm labels

---

## 🧠 Sample Brain CT Slice

The dataset consists of DICOM brain CT angiography images. Below is an example slice visualized during preprocessing.

<p align="center">
  <img src="images/normalized_dicom_slice.png" width="750">
</p>

## 🖼️ Image Preprocessing

Medical CT angiography images undergo intensity normalization and preprocessing before model training. This process standardizes pixel values across scans, reduces variability, and provides consistent inputs for the deep learning pipeline.

<p align="center">
  <img src="images/normalized_dicom_slice.png" width="750">
</p>

# ⚙️ Project Workflow

## 1. Data Loading

- Read DICOM studies
- Parse metadata
- Load expert annotations

---

## 2. Medical Image Preprocessing

- DICOM normalization
- Windowing
- Intensity scaling
- Slice ordering
- Missing value handling

---

## 3. Exploratory Data Analysis

- Patient statistics
- Class distribution
- Image dimensions
- Sample visualization
- Annotation analysis

---

## 4. Localization-aware 2.5D Input Generation

Instead of using only one CT slice, the model combines:

- Previous slice
- Current slice
- Next slice

to create richer contextual information while remaining computationally efficient.

---

## 5. Deep Learning Model

Transfer Learning using:

- EfficientNet-B0
- PyTorch
- Binary Cross Entropy Loss
- Adam Optimizer

---

## 6. Model Evaluation

Performance evaluated using:

- ROC-AUC
- Precision
- Recall
- F1 Score
- Accuracy
- Confusion Matrix
- ROC Curve
- Threshold Optimization

---

# 🧰 Technologies Used

- Python
- PyTorch
- EfficientNet-B0
- NumPy
- Pandas
- OpenCV
- pydicom
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

# 📈 Model Outputs

The notebook includes:

- Medical image visualizations
- DICOM preprocessing examples
- Localization visualization
- Training curves
- ROC Curve
- Confusion Matrix
- Prediction examples
- Clinical threshold analysis

---

# 💡 Key Learnings

This project demonstrates practical experience in:

- Medical Imaging AI
- Deep Learning
- Computer Vision
- Transfer Learning
- DICOM Processing
- Healthcare Machine Learning
- Clinical AI Evaluation
- Explainable Medical AI

---

# 🚀 Future Improvements

Potential enhancements include:

- 3D CNN architectures
- Vision Transformers (ViT)
- MONAI medical imaging framework
- Segmentation-based aneurysm localization
- Ensemble deep learning models
- Clinical deployment using TorchServe

---

# ▶️ Running the Project

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

Open

```
rsna-intracranial-aneurysm-detection-portfolio.ipynb
```

---

# 📚 References

- RSNA Intracranial Aneurysm Detection Challenge
- PyTorch Documentation
- EfficientNet Paper
- DICOM Standard

---

# 👨‍💻 Author

**Pareekshith Reddy Adla**

Healthcare AI • Medical Imaging • Computer Vision • Deep Learning • Data Science

---

⭐ If you found this repository helpful, feel free to star it!
