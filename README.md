# deep-learning-challenge

## Overview
##### A model (AlphabetSoupCharity.h5) was created in order to predict the success of future applicant buisness ventures. The model was trained on the binary success/failure history of 34,000 previous ventures and used data such as sector affiliation, government organization classification, use case, organization type, activity status, income amount, asking amount.


### Results
#### Data Preprocessing: 
##### The following data columns were utilized to train the model: APPLICATION_TYPE,	AFFILIATION,	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT. The data column IS_SUCCESSFUL was used as the target to train the model. The columns EIN and NAME were removed from the data frame because they were not relevant for training the model.
#### Compiling, Training, and Evaluating the Model
##### The model consisted of 6 hidden layers and an output layer. The hidden layers used "tanh" activation and used 6, 16, 11, 16, 6 and 21 neurons respectively for each layer. The output layer used "sigmoid" activation as is common with binary classification models. The model is able to correctly predict the success of ventures for 73% of the tested data. This falls short of the target perfomance of 75%. The parameters of the model were choosen after utilizing a tuning technique that tests various parameters in the model and reports the parameters that result in the highest accuracy. This tuning technique determined the number of layers, number of neurons, and activation type used in the model. However this technique was not successful at achieving a 75% accuracy rating for the model.

### Summary
#### Powerful techniques were utlizied to develop a neural network model to predict the success of buisness ventures. The model however did not meet the target prediction capabalities. In this assignment we were limited in developing a neural network model and excellent techniques such as implementing the kerastuner library were conducted. However, it is possible that other models might have acheieved a higher accuracy rating. Possibly a logistic regression model or random forest model might be able to achieve greater results, especially because this is a simple binary classification problem. None the less a 73% acurate neural network model is still similarly effective as a 75% accurate one, therefore this model developed in this jupyter notebook should be considered a limited success.