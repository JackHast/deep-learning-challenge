# Report

## Overview

The purpose of the analysis done in this repository is to develop a tool to help Alphabet Soup select applicants for funding that have the best chance succeeding in their ventures. The notebook "first_attempt.ipynb" is an initial attempt to create a model that has a 75 per cent prediction accuracy. Firstly, some preprocessing is done on the data set (https://static.bc-edx.com/data/dla-1-2/m21/lms/starter/charity_data.csv) from which a neural network model was created with the purpose of classifying whether an application would be successful or not based on the information provided for each applicant. In the file "AlphabetSoupCharity_Optimisation.ipynb" the are three attempts at creating a neural network that achieves 75 per cent accuracy, however, I was not able to achieve this.

## Results

### Data Preprocessing 

The target of the model, or the variable that was trying to be predicted, was whether the applicant would be successful in their venture after being funded. The data provided about each applicant 
(excluding whether they were successful or not) were therefore the features, which included, the affiliated sector of industry, government organisation classification, use case for funding, 
organisation type, active status, income classificaiton, special considerations for application and funding amount requested. There were two addition columns provided in the data set, namely,
the identification and the name of the applicant, however these columns were not seen as helpful for classification and are therefore neither targets nor features. <br>

### Compiling, Training and Evaluating the Model

Initally (code located in first_attempt.ipynb), the number of hidden layers chosen was 2 and the number of neurons were 43 (number of features), 21, 21 and 1 and the activation function 
was chosen to be the sigmoid function.

![first_model_structure](https://github.com/JackHast/deep-learning-challenge/assets/131254350/47c86e1d-4116-4f67-8474-068c7c5bc7ec)

The performance of this model fell below 75 per cent accuracy, <br

![first_model_performance](https://github.com/JackHast/deep-learning-challenge/assets/131254350/f91bbff2-9988-486c-80f9-4bacb366f1d2)

<br>

For the first attempt at optimising the model, another layer was added to the model, <br>

![second_model_structure](https://github.com/JackHast/deep-learning-challenge/assets/131254350/c9da667e-b753-4c88-bc73-abb05761016a)

However, this again fell short of the goal of 75 per cent accuracy, <br

![second_model_performance](https://github.com/JackHast/deep-learning-challenge/assets/131254350/d2bc69f9-951e-41d9-b08f-cf464fe70cdc)


For the second attempt at optimising the model, I added the same number of neurons to the two hidden layers as I did to the input layer <br>

![third_model_structure](https://github.com/JackHast/deep-learning-challenge/assets/131254350/a7af40f1-4579-4d90-bb2e-7a659cdd02e9)

Which gave, 

![third_model_performance](https://github.com/JackHast/deep-learning-challenge/assets/131254350/154cebf8-339b-45a2-a0f1-8ec4fb2ca67e)

For the final attempt at optimising the model, I didn't bin the rare values for the APPLICATION_TYPES and CLASSIFICATION columns, <br>

![fourth_model_structure](https://github.com/JackHast/deep-learning-challenge/assets/131254350/2032efcd-907a-493e-9c3d-a2a4e39d2127)

Which gave, 

![fourth_model_performance](https://github.com/JackHast/deep-learning-challenge/assets/131254350/08f6fb90-2b80-4d37-87e8-1002c85b8779)

Therefore, I was unable to successfully achieve the 75 per cent accuracy rate. 

## Summary

In conclusion, I was unsuccessful at achieving the goal of creating a model with 75 per cent accuracy. The be




                                                            


