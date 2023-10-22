# Report

## Overview

The purpose of this repository is to create a model that will help choose potential candidates for 


## Results

### Data Preprocessing 

The target of the model, or the variable that was trying to be predicted, was whether the applicant would be successful in their venture after being funded. The data provided about each applicant <br>
(excluding whether they were successful or not) were therefore the features, which included, the affiliated sector of industry, government organisation classification, use case for funding, organisation type, active status, income classificaiton, <br>
special considerations for application and funding amount requested. There were two addition columns provided in the data set, namely, the identification and the name of the applicant, however these <br>
columns were not seen as helpful for classification and are therefore neither targets or features.

### Compiling, Training and Evaluating the Model

Initally (code located in first_attempt.ipynb), the number of hidden layers chosen was 2 and the number of neurons chosen for each layer was 43 (for the input layer) which was the number of features, 

![first_model_structure](https://github.com/JackHast/deep-learning-challenge/assets/131254350/47c86e1d-4116-4f67-8474-068c7c5bc7ec)
