# Report on the Neural Network Model for Alphabet Soup

# Overview of the Analysis

The purpose of this analysis was to develop a deep learning model to predict the success of charitable donations using the dataset provided by 'Alphabet Soup.' The goal was to create a neural network model that accurately classifies whether an applivation will be successful based on various features. The model was first developed in the 'Starter_Code.ipynb' file using colab and further optimized within 'AlphabetSoupCharity_Optimization.ipynb.'

# Results

## Data Preprocessing
- The target variable 'IS_SUCCESSFUL' indicates wether or not a charity application was succesful.
- The feature variables include:
  APPLICATION_TYPE,
  AFFILIATION,
  CLASSIFICATION,
  USE_CASE,
  ORGANIZATION,
  STATUS,
  INCOME_AMT,
  SPECIAL_CONSIDERATIONS,
  ASK_AMT.
- Removing 'EIN' and 'NAME' columns from input data as they are neither targets nor features.

## Compiling, Training, and Evaluating the Model
1. Initial Model (Found in 'Starter_Code.ipynb'):
   - First Hidden Layer: 80 neurons with 'relu' activation function.
   - Second Hidden Layer: 30 neurons with 'relu' activation function.
   - Output Layer: 1 neuron with 'sigmoid' activation function.
   - Selected to balance model complexity and computational eficiency, with the 'relu' function for hidden layers to introdue non-linearity.
2. Model Preformance: Trained for 100 epochs and achieved preformance of 0.5583 Loss and 0.7280 Accuracy.
3. Steps Taken to Increase model preformance (Found in 'AlphabetSoupCharity_Optimization.ipynb'):
   - First Optimization Method was changing the amount of nodes and creating a third hidden layer with 100 neurons and 'relu' activation, this aimed to enhance the model's capacity to learn complex patterns in the data. This model trained for 100 epochs and achieved preformance of 0.5804 Loss and 0.7235 Accuracy.
   - Second Optimization Method was adding more Epochs, aiming to give the model more opportunities to learn from the data. This model trained for 200 epochs and achieved a preformance of 0.6025 Loss and 0.7241 Accuracy.
   - Third Optimization Method was changing the batch size to 55, aiming to find the optimal batch size that improves the model preformance. This model achieved a preformance of 0.5902 Loss and 0.7247 Accuracy.

# Summary

The deep learning model developed in this analysis provides a moderate level of preformancy with an initial accuary of 72.8%. After several optimization attempts, the model's accuracy was marginally improved.

## Reccomendations:

To further enhance the model's preformance:
- Experiment with more advanced achitectures or recurrent neural networks.
- Preform hyperparameter tuning using grid search or randomized search methods to find the optimal configuration.
- Consider using ensemble methods to combine multiple models and improve the accuracy of the predictions. 
