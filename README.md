# Neural_Network_Charity_Analysis

## Overview

This project’s purpose is to apply deep-learning neural networks with the TensorFlow platform in Python to analyze, and determine, which organizations classify as receiving charitable donations from Alphabet Soup’s charity.

## Results

- What variable(s) are considered the target(s) for your model?
  - The target variable that was targeted for the model was the “IS_SUCCESSFUL” category.
- What variable9s) are considered to be the features for your model?
  - The following columns were considered as features: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, and IS_SUCCESSFUL.
- What variable9s) are neither targets nor features,, and should be removed from the input data?
  - For the purpose of this model, both ‘EIN’ and ‘NAME’ columns were removed from the input data.
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - Two hidden node layers, with 80 nodes in the first layer, and the second layer included 30 neurons. Both hidden layers and the output layer included activation functions “relu” and “sigmoid”.
- Were you able to achieve the target model performance?
  - The model was not successful in obtaining the 75% accuracy target. It did, however, come in close with an accuracy of 72.3% with a loss of 57.5%.
  
  ![Accuracy_Score](https://user-images.githubusercontent.com/111096246/214365018-32dacd02-afc6-4d03-9215-7e4819f142bc.PNG)
  
- What steps did you take to try and increase model performance?
  - Changed the number of neurons in the second hidden layer from 30 to 50 neurons, and added a third hidden layer with 30 neurons. 
  
  ![third_layer](https://user-images.githubusercontent.com/111096246/214365055-213c3718-6313-4ad0-b85a-337582feabec.PNG)

## Summary

The initial model failed to meet the 75% accuracy score. After altering the model, by adding a third hidden layer and altering neuron counts in the layers, the model had a minute increase in accuracy to 72.5%. It can be concluded that by changing the number of layers, or number of neurons, the accuracy score is not heavily affected. 
A Random Forest classifier would be recommended, as it has the ability to perform binary classification, and to handle large datasets.
