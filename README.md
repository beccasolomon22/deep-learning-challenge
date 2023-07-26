# deep-learning-challenge

## Sources

1. Starter Code provided in the asssignments file
2. Stack Overflow was a great help when experiencing error messages
3. I occasionally used Chat GPT to help edit code to fix errors
4. Assignment description

   
## Overview of the analysis: 

### Background (As given in the assignment)
"The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup."

"From Alphabet Soup’s business team, you have received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as:"

* EIN and NAME—Identification columns
* APPLICATION_TYPE—Alphabet Soup application type
* AFFILIATION—Affiliated sector of industry
* CLASSIFICATION—Government organization classification
* USE_CASE—Use case for funding
* ORGANIZATION—Organization type
* STATUS—Active status
* INCOME_AMT—Income classification
* SPECIAL_CONSIDERATIONS—Special considerations for application
* ASK_AMT—Funding amount requested
* IS_SUCCESSFUL—Was the money used effectively

## Results: 

### Data Preprocessing

* What variable(s) are the target(s) for your model?

        - CLASSIFICATION and APPLICATION_TYPE
* What variable(s) are the features for your model?
  
        - IS_SUCCESSFUL
        - This is the column we are trying to train the model to predict
* What variable(s) should be removed from the input data because they are neither targets nor features?
  
        - EIN
        - These columns were dropped because they are variables that do not have a significant impact on whether a candidate is successful or not
  
### Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?
  
        - Although I tested many different amount of layers, neurons, and activation functions, these are the values I ended with
        - Layers =
        - Neurons:
              - Layer 1:
              - Layer 2:            
* Were you able to achieve the target model performance
  
        - Yes : Above 75% accuracy
* What steps did you take in your attempts to increase model performance?
  
        - Increase the number of hidden layers
        - Adjust the number of neurons on each hidden layer
        - Used Dropout to prevent overfitting
        - Try different activation functions (relu, tanh, softmax)
        - Drop additional columns that may have been contributing to lower accuracy
        - Add back in the Name column
     

## Summary: 

