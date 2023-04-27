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

## Compiling, Training, and Evaluating the Model
### How many neurons, layers, and activation functions did you select for your neural network model, and why?
### The model has five layers, including the output layer. The input layer is not explicitly defined, as its size is determined by the shape of the input data. 
* ### The first hidden layer has 80 neurons. 
* ### The second hidden layer has 40 neurons. 
* ### The third hidden layer has 30 neurons.
* ### The fourth hidden layer has 20 neurons. The output layer has a single neuron.
### The activation functions used in the model are sigmoid, relu, and linear. Sigmoid and relu are common choices for activation functions in deep neural networks, with sigmoid being useful for binary classification problems and relu being useful for general nonlinear problems. Linear activation is typically used for the output layer when predicting continuous values, such as in this regression problem.
### The number of neurons and layers in a neural network model depends on various factors, including the complexity of the problem, the size of the dataset, and the computational resources available. In this case, the number of neurons and layers was chosen based on experimentation and tuning to achieve good performance on the training and validation sets while avoiding overfitting.
![D4](https://user-images.githubusercontent.com/118647523/234758764-539db664-5bfc-4483-b102-da5eefd49cb7.png)

### Were you able to achieve the target model performance?
### The model achieved a loss of 8.2242 and an accuracy of 0.4668, which can be used as a reference for further comparison or improvement.
![D5](https://user-images.githubusercontent.com/118647523/234759086-8727f6d2-e202-435f-b631-2e5b29151cb1.png)


### What steps did you take to try and increase model performance?
### In order to improve the performance of the model, I implemented several modifications such as reducing the number of columns by dropping irrelevant features, creating additional bins to capture rare occurrences in the dataset, decreasing the bin sizes to increase the granularity of the data, increasing the number of neurons in the hidden layers to enhance the model's capacity to capture complex patterns, using different activation functions to better suit the data characteristics, and increasing the number of epochs to allow for more iterations during training. These adjustments were aimed at optimizing the model's performance by leveraging domain-specific knowledge and machine learning best practices.

## Summary 
### The given results indicate that the model achieved a loss of 8.2242 and an accuracy of 0.4668 on the validation set. The loss value is a measure of how well the model is able to minimize its errors during training, with lower values indicating better performance. The accuracy value indicates the proportion of correctly classified samples in the validation set, with higher values indicating better performance. Based on these results the accuracy is relatively low and the loss is relatively high. 

### The results suggest that further improvements to the model or alternative approaches may be necessary to achieve better performance on the task at hand. Another alternative could be a decision tree-based model such as Random Forest which have been shown to perform well on a wide range of classification problems. These models are particularly useful when dealing with datasets that have a large number of features as they can effectively handle high-dimensional data and capture non-linear relationships between the features and the target variable.
