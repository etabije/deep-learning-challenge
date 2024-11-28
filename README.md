# deep-learning-challenge

1. Overview of the Analysis
The goal of this analysis was to build a neural network to predict whether a charity application is successful or not based on certain features in the data. The task involved preprocessing the data, training a neural network, and evaluating its performance.

2. Results
Data Preprocessing

Target Variable:
The target variable (what we want to predict) is IS_SUCCESSFUL. It indicates whether an organization was successful in its application (1 for successful, 0 for unsuccessful).
Feature Variables:
The features (inputs for the model) are all the other columns that are not the target variable, such as:
APPLICATION_TYPE: Type of application (e.g., 'Individual').
CLASSIFICATION: Type of organization (e.g., 'Nonprofit').
Variables to Remove:
EIN and NAME should be removed since they don’t help predict the outcome.
Compiling, Training, and Evaluating the Model

Model Structure:
The model has 3 layers:
Input layer: Number of neurons equals the number of features.
Hidden layers: 80 neurons in the first hidden layer and 30 neurons in the second, both using ReLU activation (to help learn patterns).
Output layer: 1 neuron with sigmoid activation for binary classification (predicting success or failure).
Training:
The model was trained for 60 epochs with a batch size of 32. The model used the Adam optimizer and binary cross-entropy as the loss function.
Evaluation Results:
The model’s performance on the test set was:
Loss: 0.5672
Accuracy: 0.7251 
This means the model was able to correctly predict whether an application was successful 72% of the time.
Steps to Improve Performance:
Tried changing the number of epochs.
3. Summary
Overall Results:

The model achieved 72% accuracy on the test set, which is a solid result but can be improved and did not meet the expectation of 75%
Recommendation for Alternative Models:

Random Forests could work better for this task because they are often able to perform well with tabular data.
They also show which features are important for predictions.
