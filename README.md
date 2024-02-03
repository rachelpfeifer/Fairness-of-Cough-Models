# Explainability With Acoustic Health Data
Evaluating demographic fairness in biometric datasets.

## A Guide To This Repository:

### CoughVID Dataset
Implementing machine learning models to predict PCR test results, and then reducing bias through mitigation algorithms.
  - All files used in the analysis of the CoughVID dataset (including the original dataset itself) are in a folder called "CoughVID".
  - The original CoughVID dataset comes from the "virufy-cdf-coughvid.csv" file in a publically available repository (https://github.com/virufy/virufy-cdf-coughvid/tree/main).
  - The file called "Preprocessing CoughVID Data.ipynb" details how the original dataset was preprocessed. The preprocessed data is available in this repository in a file called "preprocessed_coughvid_dataset.csv".
  - Each audio file from the original dataset was converted to a .WAV file. The MFCC of each .WAV was extracted to include it as a feature in the machine learning model(s). The .WAV files are available by request (email: pfeifer.rachel.j@gmail.com).
