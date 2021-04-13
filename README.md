# Neural Network Charity Analysis 

## Overview of the Project
#### The purpose of this project is to use neural networks to analyze the provided dataset to create a model to predict whether an organization will be successful if funded. Using this model, Alphabet Soup will be able to make decisions about applicants trying to get funding for their charitable organizations.
 
## Results
### Data Preprocessing
* What variable(s) are considered the target(s) for your model?
	* Th target for my model is the variable ‘IS_SUCCESSFUL’.  This is the objective of the model, to determine if the organization will be successful when provided funding by Alphabet Soup.
* What variable(s) are considered to be features for your model?
	* The variables that are considered to be features for the model are: ‘APPLICATION_TYPE’, ‘AFFILIATION’, ‘CLASSIFICATION’, ‘USE_CASE’, ‘ORGANIZATION’, ‘STATUS’, ‘INCOME_AMT’,  ‘SPECIAL_CONSIDERATIONS’, and ‘ASK_AMT’.
* What variable(s) are neither targets nor features, and should be removed from the input data?
	* ‘EIN’ and ‘NAME’ were removed from the data.  They are simply identification columns and have no bearing on the analysis to be performed.

### Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
	* The input layer has nodes equal to the number of features.
	* I chose to have 2 hidden layers, the first with 80 nodes because it is about double the number of features.  The second layer had 30 nodes. I used the relu function for the hidden layers as it is the default activation function to begin.
	* For the output layer, I chose the sigmoid activation function because we were looking at a binary classification.
* Were you able to achieve the target model performance?
	* No, I was not able to achieve the target model performance of 75%
* What steps did you take to try and increase model performance?
	* To try to increase ethe model performance, I tried various tweaks to the model.  I tried removing an additional feature, changed the number of nodes in the hidden layers, changed the number of hidden layers, and changed the number of epochs.
	
## Summary 
#### After making several attempts, I was unable to improve the model to at least a 75% accuracy rate. The many changes I made to the model decreased the accuracy rate.  Because these various tweaks that I made only served to decrease the result, I would recommend using a different model to see if the results could be improved.  In particular, I would try the SVM model because it works very well as a binary classifier.
