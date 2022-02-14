# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis was to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results
###Data Processing

-The target for the model is the success of the applicants displayed in the "IS_SUCCESSFUL" column.

-The following variables are the features of the model:
    APPLICATION_TYPE
    AFFILIATION
    CLASSIFICATION
    USE_CASE
    ORGANIZATION
    INCOME_AMT
    SPECIAL_CONSIDERATIONS

-The variables EIN and Name were neither targets nor features, and were removed from the input data.

###Compiling, Training, and Evaluating the Model

-In my first attempt to optimize the model, I added more neurons to the 2 hidden layers, the first containing 100 nuerons, and the second containing 40 neurons. The activation function used for all layers was "relu".

![picture alt](https://github.com/ChristinaGalley/Neural_Network_Charity_Analysis/blob/main/Resources/adding_neurons.png)

-This first optimization only achieved a model performance of 72.5%.

![picture alt](https://github.com/ChristinaGalley/Neural_Network_Charity_Analysis/blob/main/Resources/attempt_1_accuracy.png)

-Next, I added a third hidden layer and adjusted the neurons per layer. This resulted in a slight decrease in accuracy to 72.4%.

![picture alt](https://github.com/ChristinaGalley/Neural_Network_Charity_Analysis/blob/main/Resources/attempt_2_accuracy.png)

-Lastly, I using a different activation function (tanh) for the hidden layers. This, again, resulted in an accuracy of 72.4%.

![picture alt](https://github.com/ChristinaGalley/Neural_Network_Charity_Analysis/blob/main/Resources/attempt_3_accuracy.png)

## Summary
At the end, I was not able to optimize the accuracy of the model to the targeted 75%. Despite 3 atempts to optimize the model, no attempt resulted in an increase in the accuracy compared to the orignial model yeilding a 72.6% accuracy.

![picture alt](https://github.com/ChristinaGalley/Neural_Network_Charity_Analysis/blob/main/Resources/original_model_accuracy.png)

To solve this classification problem, I would recommend trying a different model. An SVM model may be a better design to classify the data into 2 classes: applicant success, or failure. Another model to trial would be Random Forest Classifier, which could prevent possible overfitting.