# CognoRise_Internship

## Task 1: Data Preprocessing and Classification for Breast Cancer Data
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


# Task 7: Convolutional Neural Network for MNIST Classification
Steps:
### - Data Preparation:

  Loaded the MNIST dataset and reshaped the data for a CNN model.
  Normalized pixel values to the range [0, 1].
### - Model Definition:

  Built a sequential CNN model with:
  Two convolutional layers (32 filters, 3x3 kernel) and ReLU activation.
  Max pooling layers.
  Flattening layer followed by a dense layer with softmax activation.

### - Model Compilation and Training:

  Compiled the model using the Adam optimizer and Sparse Categorical Crossentropy loss.
  Trained the model for 2 epochs with a batch size of 128.
  Achieved an accuracy of 97.27% on the training set.
### - Model Evaluation:

  Evaluated the model on the test set, obtaining an accuracy of 97.90%.
### - Model Summary:

  Total parameters: 17,578 (all trainable).


# Task 8: Twitter Emoji Prediction Model

### Steps:

1. **Data Import and Merging**:
   - Loaded Twitter emoji dataset and emoji mapping.
   - Merged datasets to associate text with corresponding emojis.

2. **Exploratory Data Analysis**:
   - Plotted frequency of emojis used in tweets.

3. **Text Preprocessing**:
   - Lowercased text, removed URLs, mentions, hashtags, and special characters.
   - Tokenized and lemmatized text using NLTK.

4. **Tokenization and Padding**:
   - Tokenized cleaned text, converting it to sequences.
   - Padded sequences to a maximum length of 50.

5. **Word2Vec Embedding**:
   - Trained Word2Vec model on tokenized sentences.
   - Created an embedding matrix for model input.

6. **Class Weights Calculation**:
   - Computed class weights to handle class imbalance.

7. **Train-Test Split**:
   - Split data into training and test sets, including sample weights.

8. **Model Definition**:
   - Built a Bidirectional LSTM model with Multi-Head Attention:
     - Input layer, embedding layer, LSTM layer, Batch Normalization, Dropout, and Dense output layer.

9. **Model Compilation and Training**:
   - Compiled model with Adam optimizer and sparse categorical crossentropy loss.
   - Trained the model for 50 epochs, achieving good validation accuracy.

10. **Model Architecture (5 Classes)**:
    - Adjusted the architecture to predict 5 classes.
    - Achieved a total of **17,453,417** parameters in the final model.

