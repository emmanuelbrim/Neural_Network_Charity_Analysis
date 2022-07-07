# Neutral_Network_Charity_Analysis
_Using Machine Learning to Predict Success of a Charity's Investment_

## Overview of the analysis
Alphabet Soup, an organization engaged in the funding of charitable endeavours seeks to realize the best outcome of all their investments.
The project was to help Beks of Alphabet Soup develop a machine learning model based on neural networks which uses binary classification to predict if an  organization will be successful or not when sponsored.

## Results
The analysis involved the use of data from Alphabet Soup's business team. The CSV document entailed information on 34,000 organizations that have received funding from Alphabet Soup.

- Data Preprocessing

  - A column labeled 'IS_SUCCESSFUL' in the tabular dataset showed whether an organization was successful or not upon sponsorship.
  Since this tells the outcome of funding or whether the money was used effectively, this variable therefore served as the target for the model's predictions.
  
  - Upon review of the remaining metadata on the organizations, nine other data points were determined as input variables for the model. 
  The following variables were used as the features for the model.
  
    APPLICATION_TYPE,
    
    AFFILIATION,
    
    CLASSIFICATION,
    
    USE_CASE,
    
    ORGANIZATION,
    
    STATUS,
    
    INCOME_AMT,
    
    SPECIAL_CONSIDERATIONS,
    
    ASK_AMT
    
  - The remaining columns; 'EIN' and 'NAME' served as unique identifiers for the applying organizations and therefore did not have any bearing on predicting the   outcome of funding. Hence both variables were not included in the model. 

- Compiling, Training, and Evaluating the Model

  - The initial Deep-learning Neural Network involved 43 input features after encoding all the categorical features.
  As a deep learner, two hidden layers was used in the inital persuit. 
  In an attempt to boost training, twice the amount of input(80 neurons) was used in the first layer. The second layer had 30 neurons and a single neuron for   the output layer. 
  The Relu function was used to activate the first and second layers.
  As a binary classifier the Sigmoid function was the best to be used to activate the output layer. 
  
  - The model could not achieve the target performance. The accuracy after evaluation was below 75%.
  
  - There was no significant improvement to the initial model performance of 72.73% after several efforts to optimize the model.
  
    To improve performance the following steps were taken;
    
      Reshaped the features variables by removing the 'STATUS' column
      ![]()
      
      Applied more bining on the 'APPLICATION TYPE" feature.
      ![]()
      
      Increased the hidden layers for the model.
      ![]()
      
      Changed the optimizer for compiling the model. 
      ![]()
      
     The final performance of the model to predict outcomes showed an accuracy of 72.85%.

## Summary

The model didnot achieve the target accuracy of 75% or more after attempts at improving it.
It is however recommended that additional data might change the results since the model was tuned only on what was available.
The fact that a Deep-Learning model could not achieve the desired results doesnot also mean that it is not achievable. An alternative will be compare performance of this model with an other machine learning model like RandomForestClassifier to evaluate performance.
