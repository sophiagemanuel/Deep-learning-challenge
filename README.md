# Report on the Neural Network Model for Alphabet Soup

# Overview of the Analysis

The purpose of this analysis was to develop a deep learning model to predict the success of charitable donations using the dataset provided by 'Alphabet Soup.' The goal was to create a neural network model that accurately classifies whether an applivation will be successful based on various features. The model was first developed in the 'Starter_Code.ipynb' file using colab and further optimized within 'AlphabetSoupCharity_Optimization.ipynb.'

# Results

## Data Preprocessing
- The target variable 'IS_SUCCESSFUL' indicates wether or not a charity application was succesful.
- The feature variables include:
  APPLICATION_TYPE
  AFFILIATION
  CLASSIFICATION
  USE_CASE
  ORGANIZATION
  STATUS
  INCOME_AMT
  SPECIAL_CONSIDERATIONS
  ASK_AMT
- Removing 'EIN' and 'NAME' columns from input data as they are neither targets nor features.
