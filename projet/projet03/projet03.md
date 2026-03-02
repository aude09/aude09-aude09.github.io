# Alzheimer MRI Classification using 3D Deep Learning
**Year:** 2025  
**Category:** Medical AI / Deep Learning / Neuroimaging  
**Status:** Research Project – Stable Experimental Version  

## Project Overview
This project focuses on the classification of Alzheimer’s disease stages using 3D brain MRI data and deep learning techniques.

The objective is to automatically classify patients into three clinical categories:

- Cognitively Normal (CN)
- Mild Cognitive Impairment (MCI)
- Alzheimer’s Disease (AD)

A 3D Convolutional Neural Network (CNN) is trained on preprocessed MRI volumes to learn spatial brain patterns associated with disease progression.

This project was developed for educational and research purposes and is not intended for clinical use.

---

## Dataset

The MRI data were obtained from the Alzheimer's Disease Neuroimaging Initiative (ADNI) database.

For this project, 3T MRI scans from **ADNI1: Complete 3Y 3T** were used to ensure higher spatial resolution and longer longitudinal consistency.

Access the dataset here:
https://adni.loni.usc.edu/data-samples/adni-data/neuroimaging/mri/mri-image-data-sets/

To download the data:
1. Create an ADNI account.
2. Follow the official data access instructions.
3. Ensure sufficient storage capacity before downloading (MRI volumes are large).

---

## Methodology

### 1. Data Preparation
- Loading MRI volumes in NIfTI format
- Matching MRI scans with clinical metadata
- Label encoding (CN = 0, MCI = 1, AD = 2)

### 2. Preprocessing
- Intensity normalization
- Resizing / spatial alignment
- Optional skull stripping (if applied)
- Conversion to tensor format

### 3. Dataset Construction
- Custom PyTorch Dataset class
- Efficient 3D data loading pipeline

### 4. Model Development
- 3D Convolutional Neural Network (CNN)
- Training with cross-entropy loss
- Performance monitoring across epochs

### 5. Evaluation
- Classification accuracy
- Confusion matrix
- Overfitting monitoring

---

## Technologies & Tools
- Python
- PyTorch
- NumPy
- Pandas
- Scikit-learn
- NiBabel
- SciPy
- Jupyter Notebook / VS Code

---

## Execution Time
Due to the size of 3D MRI volumes and the computational cost of 3D CNNs, preprocessing and training may take several hours depending on hardware resources (CPU vs GPU).

GPU acceleration is strongly recommended.

---

## Future Improvements
- Data augmentation for 3D volumes
- Transfer learning with medical pretrained models
- Cross-validation on larger subsets
- Integration with clinical feature prediction
- Model explainability (Grad-CAM for 3D)

---

## Visualizations
![MRI Example](../assets/images/mri_sample.png)
![Training Accuracy](../assets/images/training_curve_mri.png)

---

## License
MIT License

---

## Disclaimer
This project is for research and educational purposes only and is not intended for clinical diagnosis.
