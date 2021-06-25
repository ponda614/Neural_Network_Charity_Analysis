# Overview of the analysis

- With the knowledge of machine learning and neural networks, I used the features in the provided dataset to help Beks create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.From Alphabet Soup’s business team, Beks received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organization classification
USE_CASE—Use case for funding
ORGANIZATION—Organization type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special consideration for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

# Results

## Data Preprocessing

What variable(s) are considered the target(s) for your model?

- The column IS_SUCCESSFUL has binary data referencing whether or not the charity donations was used effectively and is considered the target for our deep learning neural network. 

What variable(s) are considered to be the features for your model?

- The following columns APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT are considered the features for our model.

What variable(s) are neither targets nor features, and should be removed from the input data?

- EIN and NAME are identification information and have been removed from the input data.

## Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

- layer1 = 80 with activation="relu", layer2 = 30 with activation="relu", Outer layer activation = "sigmoid"

Were you able to achieve the target model performance?

- No, we were not able to achieve the target model performance because we had 
Loss: 0.5573652386665344, Accuracy: 0.7257142663002014

What steps did you take to try and increase model performance?

- I added a third hidden laer but it decreased the accuracy. We also increased the number of neurons in one of the hidden layer but it also showed no improvements in accuracy 

# Summary 

- The model does not reach the target of 75% accuracy and hits a limit of 73% accuracy with few optimization efforts.

- Random Forest Classifier can be used to solve the classification issue because we are in a binary classification situation. 