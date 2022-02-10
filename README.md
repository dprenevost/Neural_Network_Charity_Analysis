# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis is to use Neural Network models to predict whether applicants will be successful if they are funded by Alphabet Soup.

Data Preprocessing
The target for the model is "IS_SUCCESSFUL" i.e. whether the applicants will be successful or not.
The "EIN" and "Name" of the applicants are neither features nor targets and are dropped during preprocessing.


Compiling, Training and Evaluating the Model
In trying to optimize the model, a variety of number of neurons, layers and activation functions are tested. They are listed below:
Optimization #1:
Two hidden layers are used with 80 and 10 neurons respectively
The ReLu activation function is used for the two hidden layers
The sigmoid activation function is used for the output layer

![optimize1](https://user-images.githubusercontent.com/91210001/153321678-3612eb9e-1e0c-4bee-92f0-07574927543e.PNG)

Optimization #2:
Two hidden layers are used with 160 and 50 neurons respectively
The ReLu activation function is used for the two hidden layers
The sigmoid activation function is used for the output layer


Optimization #3:
Three hidden layers are used with 80, 30, and 10 neurons respectively
The ReLu activation function is used for the hidden layers
The tanh activation function is used for the output layer


The target model accuracy of 75% was not achieved despite the changes described above and in addition to the following changes made to the original model:

Summary
Using the original model, an accuracy of 72.7% was achieved


![model](https://user-images.githubusercontent.com/91210001/153322007-c3566b3f-dc7b-4213-92a6-8aae0535b876.PNG)

Optimization #1 had the next highest accuracy rate of 72.4% followed by Optimization #2 (70.8%) and Optimization #3 (61.7%)

Recommendation
It does not appear that adding more layers, neurons and epochs improve the accuracy. The next iteration recommended is as follows:

Use the bins for Application Types and Classification as the numbers in one category in each of the Application Types and Classification are very large compared to the rest of the bins. This will hopefully get rid of the outliers.
Keep to two hidden layers with 80 and 30 neurons respectively 
Keep to the sigmoid activation function for the output layer 
Alternatively, the SVM model can be trialed to determine if a comparable or better accuracy rate can be achieved. SVM is designed to classify data into two classes. 
