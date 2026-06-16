# Methods

## Dataset

This project uses the PTB-XL public electrocardiography dataset. For the baseline pipeline, the 100 Hz waveform files were used. Metadata and diagnostic label information were loaded from the provided PTB-XL CSV files.

## Label Definition

A binary classification task was defined:
- normal
- abnormal

An ECG recording was labeled as normal if its SCP code dictionary contained `NORM`. All other recordings were labeled as abnormal.

## Waveform Processing

Individual ECG recordings were loaded using the waveform file paths provided in the PTB-XL metadata table. The low-resolution waveform files (`filename_lr`) were used for the baseline version of the project.

## Feature Extraction

For each of the 12 ECG leads, the following basic signal features were extracted:

- mean
- standard deviation
- minimum
- maximum
- root mean square (RMS)

This produced a structured feature table used for classification.

## Model

A random forest classifier was used as the baseline model. The feature table was split into training and test sets using an 80/20 split with stratification by class.

## Evaluation

The model was evaluated using:
- accuracy
- precision
- recall
- F1-score
- ROC-AUC
- confusion matrix

Additional outputs included feature importance ranking and example ECG waveform plots.