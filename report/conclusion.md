# Conclusion

This project developed a baseline dry-lab biomedical engineering pipeline for classifying 12-lead ECG recordings as normal or abnormal using the PTB-XL dataset.

The current system successfully loads waveform data, extracts simple signal features, trains a random forest classifier, and generates evaluation outputs including a confusion matrix, ROC curve, class distribution plot, and feature importance analysis.

The baseline results show that even simple engineered features can support meaningful discrimination between normal and abnormal ECG recordings. This makes the project a strong foundation for future extensions.

Future work will expand the system beyond binary classification to predict broader ECG abnormality categories such as MI, STTC, CD, and HYP, and later support finer-grained diagnostic prediction and stronger explainability methods.