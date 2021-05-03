# Neural_Network_Charity_Analysis

## Overview
The purpose of this analysis is to perform a Deep Learning Neural Network analysis using data on 34,000 organizations that have received funding from Alphabet Soup. Our team decided to use TensorFlow platform in Python via Jupyter Notebook for our initial analysis. Our analysis aims to predict which charities were successful with a target accuracy score of 75%.

## Results
Data Preprocessing
* Target variable: 'IS_SUCCESSFUL' column
* Feature variables: 'APPLICATION_TYPE', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT','SPECIAL_CONSIDERATIONS', and 'ASK_AMT'
* Dropped variables: "EIN" and "NAME" columns were removed because they don't provide any useful information to the model

Compiling, Training, and Evaluating the Model
- Number of Neurons, layers, and activation function: I decided to choose two hidden layers with 80 neurons in the first layer and 30 neurons in the second layer. This is based on general rule of thumb of using 2 to 3 times the number of features. The activation function was "Relu", however, in later parts of the project trial and error was using to determine better activation function that is better fits the model.
- Accuracy score: After several improvements and attempts, the revised model was able to have an accuracy score of 71.9% which is short from the target of 75%.
- Steps to improve model accuracy:
    1) Added more neurons per layer
    2) Added more hidden layers
    3) Attempted several changes to activation function 
  <img src="/Resources/Images/ModelSummary.png"/>

## Summary
In Summary, the revised model was able to achieve an accuracy score of about 72% which is short of our target of 75%. Upon making several attempts to improve the accuracy, it was apparent that increasing the number of neurons and hidden layers had diminishing returns and was not able to further improve the model accuracy after certain threshold. Also, the extremely high number of hidden layers and neurons may cause overfitting issues. Therefore, it is recommended to first try to identify whether the current model is overfitted. Also, another recommendation for future analysis is to consider balanced random forest ensamble model.
