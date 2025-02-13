deep-learning-challenge ---- Neural Network Model Report for Alphabet Soup

          Overview of the Analysis:

The purpose of this analysis is to develop a deep learning model using a neural network to predict whether applicants for funding from Alphabet Soup will be successful. 


         --- Data Preprocessing

======= Target Variable: "IS_SUCCESSFUL" - variable indicates whether an applicant was successful (1) or not (0).

======= Feature Variables: "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT" 

======= Removed Variables: "EIN" and "NAME" were dropped because they are unique identifiers and do not contribute to the predictive model.

          --- Compiling, Training, and Evaluating the Model

          Model Architecture:

=======   Input Layer: 
          Number of neurons equal to the number of features.

=======   Hidden Layers:
          First hidden layer: 80 neurons, relu activation function
          Second hidden layer: 30 neurons, relu activation function

========  Output Layer:
          1 neuron with sigmoid activation function

========  Optimizer: 
          Adam

========  Loss function: 
          Binary Crossentropy

         
          Performance Results:

Initial model accuracy: ~72%



          Attempts to Improve Model Performance:

Increased the number of neurons and layers:
          First hidden layer: 128neurons, relu activation function
          Second hidden layer: 64 neurons, relu activation function
          Third hidden layer: 32 neurons, relu activation function

Experimented with different activation functions (ReLU performed best)

Summary

The deep learning model achieved moderate accuracy (~73%), which may not be sufficient for making highly reliable funding decisions.

          Alternative Model Recommendation:

Given the structured nature of the dataset, a different model might yield better results
Increasing the number of epochs and decreasing the batch size might yield better results

