# Results

## Binary Classification Performance

A baseline random forest classifier was trained on extracted ECG features from 1,000 PTB-XL recordings to distinguish normal and abnormal ECGs.

The model achieved the following performance:

- Accuracy: 0.73
- Precision (abnormal): 0.71
- Recall (abnormal): 0.72
- F1-score (abnormal): 0.72
- ROC-AUC: 0.814

## Generated Outputs

The current baseline pipeline produced the following result artifacts:

- confusion matrix
- ROC curve
- feature importance plot
- class distribution plot
- example ECG waveform plots
- saved feature importance table
- saved classification report
- saved metrics summary table

## Interpretation

The baseline results show that simple engineered ECG features combined with a random forest classifier can provide meaningful separation between normal and abnormal ECG recordings. The ROC-AUC above 0.8 suggests that the model captures useful signal-level differences, even with a relatively simple feature set and a limited subset of the full dataset.

## Current Limitation

This version performs binary classification only and does not yet distinguish among abnormality subtypes such as MI, STTC, CD, or HYP.