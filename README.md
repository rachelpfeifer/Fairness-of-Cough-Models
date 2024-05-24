# Fairness of Cough Models
Evaluating demographic fairness in biometric datasets. Implementing machine learning models to predict COVID-19 test results, and then reducing bias through mitigation algorithms.

## A Guide To This Repository:
Two datasets, Coswara and CoughVID, were analyzed. Each dataset is in its respective folder given by the name of the dataset (Coswara and CoughVID). For each dataset, there are sub-folders for the analysis, figures, and results.

The Analysis folder contains the analyses for the demographic parity and equalized odds based on the results obtained for both gender and age. The .ipynb file for demographic parity contains calculations for the average selection rate before mitigation vs. after mitigation, percent improvement calculations for both the demographic parity ratio and demographic parity difference, and Student's/Welch's Two-sample t-tests for the demographic parity difference. The .ipynb file for equalized odds contains calculations for the average false negative rate before mitigation vs. after mitigation, percent improvement calculations for both the equalized odds ratio and the equalized odds difference, and Student's/Welch's Two-sample t-tests for the equalized odds difference.

The Figures folder has the two .ipynb files that contain the code that produces the figures for demographic parity and equalized odds. The code generates 12 figures for each dataset (3 for demographic parity for gender, 3 for demographic parity for age, 3 for equalized odds for gender, and 3 for equalized odds for age).

The Results folder includes two .ipynb files. One .ipynb file is the code for the decision tree model (based on the parameters returned from grid search cross-validation) that is used to produce the metric values for demographic parity before and after mitigation for gender and age (this is repeated for a total of 30 iterations for gender and 30 iterations for age). The other .ipynb file contains the code that is used for the decision tree model (based on the parameters returned from grid search cross-validation) to determine the metric values for equalized odds before and after mitigation for gender and age (this is repeated for a total of 30 iterations for gender and 30 iterations for age).


### Coswara Dataset
As mentioned above, the Coswara dataset is divided into 3 sub-folders: Analysis, Figures, and Results. The original Coswara dataset comes from a publically available repository (https://github.com/iiscleap/Coswara-Data). The audio files (in .WAV format) used while preprocessing the original dataset are available in the previously mentioned repository (https://github.com/iiscleap/Coswara-Data). The MFCC of each of these .WAV files was extracted to use as a feature in the machine learning model(s).


### CoughVID Dataset
The CoughVID dataset is split into 3 sub-folders: Analysis, Figures, and Results. The original CoughVID dataset comes from the publically available repository (https://github.com/virufy/virufy-cdf-coughvid/tree/main). Each audio file from the original dataset was converted to a .WAV file, and the MFCC of each .WAV was extracted to include it as a feature in the machine learning model(s).
