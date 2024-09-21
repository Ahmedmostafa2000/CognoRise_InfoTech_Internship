# CognoRise_Internship

## Task 1: Data Preprocessing and Classification with KNN
Steps:
### - Data Loading and Preprocessing:

  Loaded the dataset using pandas.
  Removed unnecessary columns and encoded the diagnosis column (Malignant = 1, Benign = 0).
  Separated features (X) and target (y).

### - Exploratory Data Analysis:

  Generated a correlation heatmap to identify feature relationships.
  Created a bar plot to visualize the count of Malignant and Benign cases.
### - Modeling:

  Split the data into training and testing sets.
  KNN classifiers for values of k (2-6).
  Reported highest accuracy, confusion matrix, and classification metrics for each k.
  Achieved the highest accuracy of 95.6% with k=5.
