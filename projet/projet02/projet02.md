# Voice Emotion Recognition using Machine Learning
**Year:** 2025  
**Category:** Artificial Intelligence / Audio Signal Processing / Machine Learning  
**Status:** In Progress – Stable Version

## Project Overview
This project focuses on detecting human emotions from speech using machine learning techniques.

The goal is to analyze vocal characteristics in order to classify emotional states from audio recordings. The system processes raw audio data, extracts relevant acoustic features, and trains a classification model capable of recognizing different emotions.

This work was developed as part of a personal learning and research initiative in Artificial Intelligence.

## Methodology

### 1. Audio Preprocessing
- Signal cleaning
- Normalization
- Segmentation of audio samples

### 2. Feature Extraction
- MFCC (Mel-Frequency Cepstral Coefficients)
- Spectrogram analysis
- Chroma features
- Zero-crossing rate

### 3. Data Augmentation
- Noise injection
- Pitch shifting
- Time stretching

### 4. Model Training
- Classical machine learning models (Scikit-learn)
- Performance optimization
- Evaluation using classification metrics

## Technologies & Tools
- Python
- Librosa
- NumPy
- Pandas
- Scikit-learn
- Jupyter Notebook / Google Colab

## Dataset
This project is based on publicly available datasets from Kaggle.

Source:  
https://www.kaggle.com/datasets

The implementation was adapted and extended as part of a personal learning project.

## Execution Time
Depending on hardware specifications, feature extraction and model training may take several hours. Long execution times are expected on standard personal computers.

## Future Improvements
- Implementation of Deep Learning models (CNN / RNN)
- Real-time emotion recognition
- Deployment as an interactive application

## Visualizations
![Spectrogram Example](../assets/images/spectrogram.png)
![Training Performance Curve](../assets/images/training_curve.png)
