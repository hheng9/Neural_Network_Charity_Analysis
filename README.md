# Neural_Network_Charity_Analysis

## Overview of the loan prediction risk analysis
### This analysis involves creating a binary classifier using a dataset of 34,000 organizations that received funding from Alphabet Soup. The goal is to preprocess the data, compile, train, and evaluate a neural network model to predict if an applicant will be successful. The article discusses the differences between traditional machine learning classification, regression models, neural network models, perceptron model, and algorithm performance. We use TensorFlow to create and train machine learning models, particularly neural networks, with a flexible and efficient architecture, and to deploy them on various platforms.

## Results 
### What variable(s) are considered the target(s) for your model?
* ### The "IS_SUCCESSFUL" column is considered to be the target for my model.
![D1](https://user-images.githubusercontent.com/118647523/234757154-853962c6-efac-4e9f-ad6f-6075c3167778.png)

### What variable(s) are considered to be the features for your model?
* ### The APPLICATION_TYPES, AFFILIATION, USE_CASE, ORGANIZATION, INCOME AMOUNT, AND ASK_AMT are considered to be the features for my model.
![D2](https://user-images.githubusercontent.com/118647523/234757873-eeae1b39-7512-4439-a6ab-8a6b0064f943.png)

### What variable(s) are neither targets nor features, and should be removed from the input data?
* ### The EIN, NAME, CLASSIFICATION, SPECIAL_CONSIDERATIONS columns are not target and have been removed from the input data.
![D3](https://user-images.githubusercontent.com/118647523/234758142-b89bd3a4-bd3d-4d98-b98d-ffe5a19036b3.png)

##Compiling, Training, and Evaluating the Model
### How many neurons, layers, and activation functions did you select for your neural network model, and why?
### Were you able to achieve the target model performance?
### What steps did you take to try and increase model performance?
