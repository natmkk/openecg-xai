# Introduction

Electrocardiography is one of the most common noninvasive tools used to evaluate cardiac electrical activity. Because ECG recordings are widely used in clinical settings, automated analysis of ECG signals is an important biomedical engineering problem.

This project focuses on building a dry-lab computational pipeline for ECG classification using the PTB-XL public dataset. The baseline goal is to classify 12-lead ECG recordings as normal or abnormal using extracted signal features and a machine learning model.

In addition to classification, the project emphasizes interpretability and reproducibility. The workflow includes waveform visualization, feature extraction, model evaluation, and feature importance analysis, making the system useful both as an engineering prototype and as an open-source educational project.

The current version is limited to binary classification, but it is designed to support future extensions to broader abnormality-category prediction and more detailed diagnostic classification.