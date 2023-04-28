# -Neural_Network_Charity_Analysis
Module 20 - Neutral Networks
## Overview of the analysis: Explain the purpose of this analysis.
With the use of machine learning and neural networks, we will create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The datset contains a number of columns that capture metadata about each organization, such as the following:
---
•	EIN and NAME—Identification columns
•	APPLICATION_TYPE—Alphabet Soup application type
•	AFFILIATION—Affiliated sector of industry
•	CLASSIFICATION—Government organization classification
•	USE_CASE—Use case for funding
•	ORGANIZATION—Organization type
•	STATUS—Active status
•	INCOME_AMT—Income classification
•	SPECIAL_CONSIDERATIONS—Special consideration for application
•	ASK_AMT—Funding amount requested
•	IS_SUCCESSFUL—Was the money used effectively
We will process, compile, and optimize to neutral network model. 

## Results: 
### Data Preprocessing
---
When processing the model, we will clean up the data, examine unique values, create density plots, use one-hot coding, scale the data, and much more.
---
•	What variable(s) are considered the target(s) for your model?
o	The targets that are stated to be successful in the dataset, which ultimately means it has been funded by the AlphabetSoup.
•	What variable(s) are considered to be the features for your model?
o	The feature in the dataset is the ‘IS_SUCCESSFUL” column.
•	What variable(s) are neither targets nor features, and should be removed from the input data?
o	The EIN and NAME columns are neither targets nor features, which is why we have removed them from the dataset.
---
![Classification_Type_Density](https://user-images.githubusercontent.com/119131202/235037694-d595cdd6-d05d-4b91-9d2b-4893a179d174.PNG)

### Compiling, Training, and Evaluating the Model
---
When compiling the model, we will utilize tensorflow keras, create layers, analyze the model structure, train the model, create a callback, and evaluate the model using test data.
---
•	How many neurons, layers, and activation functions did you select for your neural network model, and why?
o	We used 4 layers, each with a different number of neurons. The first layer had 110 neurons with relu activation. The second layer had 80 neurons with the relu activation. The third layer had 40 neurons with sigmoid activation. The last layer had 20 neurons with sigmoid activation. Different activation style work better with different amount of neutrons.
•	Were you able to achieve the target model performance?
o	No, the model had 71.3% accuracy, but the target model performance goal was 75%.
•	What steps did you take to try and increase model performance?
o	The STATUS and SPECIAL_CONSIDERATIONS columns were removed when trying to increase model performance. Additionally, the number of neurons and layers were increased. Lastly, we tried different combinations of activations styles with the model, but the relu activation was most successful.

## Summary

To optimize the model performance, the testing suggests that you should utilize the relu activation, with many neurons and layers. The classification problem could possibly be solved by creating a model using the random forest classifier to help with the influence of outliers.
---
Analyis Performed by Katelin Catton
2/27/2023
