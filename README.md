deep-learning-challenge ---- Neural Network Model Report for Alphabet Soup

Overview of the Analysis

The purpose of this analysis is to develop a deep learning model using a neural network to predict whether applicants for funding from Alphabet Soup will be successful. 

Results:

--- Data Preprocessing

* Target Variable: "IS_SUCCESSFUL" - variable indicates whether an applicant was successful (1) or not (0).

* Feature Variables: "APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT" 

* Removed Variables: "EIN" and "NAME" were dropped because they are unique identifiers and do not contribute to the predictive model.

--- Compiling, Training, and Evaluating the Model

Model Architecture:

=======   Input Layer: 
          Number of neurons equal to the number of features.

=======   Hidden Layers:
          First hidden layer: 80 neurons, relu activation function
          Second hidden layer: 30 neurons, relu activation function

Output Layer:

1 neuron with sigmoid activation function (since this is a binary classification problem)

Performance Results:

Initial model accuracy: ~72-73%

Loss function: Binary Crossentropy

Optimizer: Adam

Attempts to Improve Model Performance:

Increased the number of neurons and layers

Experimented with different activation functions (ReLU performed best)

Summary

The deep learning model achieved moderate accuracy (~73%), which may not be sufficient for making highly reliable funding decisions.

Alternative Model Recommendation:

Given the structured nature of the dataset, a different model might yield better results:

Random Forest Classifier:

It handles categorical variables effectively and is less prone to overfitting.

Provides feature importance insights, helping identify the most critical factors for predicting success.

XGBoost (Extreme Gradient Boosting):

Final Recommendation:
While the deep learning model provided useful insights, a tree-based model like XGBoost or Random Forest should be tested for potential performance improvements.

