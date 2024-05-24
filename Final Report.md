# Report on the Neural Network Model for Alphabet Soup

## Overview of the Analysis

The purpose of this analysis was to develop a binary classifier using machine learning and neural networks to predict the success of applicants funded by the nonprofit foundation Alphabet Soup. By analyzing historical data on organizations that have received funding, the goal was to identify features that correlate with successful outcomes and build a model that could aid Alphabet Soup in selecting the most promising applicants for future funding.

## Results

### Data Preprocessing

**Target Variable:**
- `IS_SUCCESSFUL`: This variable indicates whether the funding was used effectively, and was the target for the binary classification model.

**Feature Variables:**
- `APPLICATION_TYPE`: Alphabet Soup application type
- `AFFILIATION`: Affiliated sector of industry
- `CLASSIFICATION`: Government organization classification
- `USE_CASE`: Use case for funding
- `ORGANIZATION`: Organization type
- `STATUS`: Active status
- `INCOME_AMT`: Income classification
- `SPECIAL_CONSIDERATIONS`: Special considerations for application
- `ASK_AMT`: Funding amount requested

**Variables Removed:**
- `EIN`: Identification number, not relevant for the model.
- `NAME`: Name of the organization, not relevant for the model.

### Compiling, Training, and Evaluating the Model

**Model Architecture:**
- **Input Layer:** The number of input features was determined by the number of columns after preprocessing.
- **Hidden Layers:**
  - **First Hidden Layer:** `10` neurons (where 10 was chosen based on the input features), with a `ReLU` activation function to handle non-linearity.
  - **Second Hidden Layer:** `10` neurons (where 10 was chosen to balance model complexity and performance), with a `ReLU` activation function.
- **Output Layer:** 1 neuron with a `sigmoid` activation function to produce a binary output.

![Model Architecture](Images/Initial_Model_Architecture.png)

![Model Overview](Images/Initial_Model_Overview.png)

**Model Performance:**
- **Initial Performance:** The initial model's accuracy and loss metrics were evaluated on the test dataset.
- **Target Performance:** The goal was to achieve an accuracy higher than 75% but the accuracy was calcualted to be 0.7246 or ~72.5%.

![Initial Results](Images/Initial_Results.png)

**Optimization Attempts:**
1. **Adjusting Input Data:**
   - The Name Column was no longer dropped but instead all names with a count of < 45 were grouped as 'Other'
2. **Model Architecture:**
   - The number of neurons in the hidden layers was increased.
   - An additional hidden layer was added.
3. **Training Regimen:**
   - The number number of epochs was increased to 100 allow more training iterations.
   
![Optimized Model Architecture](Images/Optimized_Model_Architecture.png)

![Optimized Model Overview](Images/Optimized_Model_Overview.png)

**Final Model Performance:**
- The final model achieved an accuracy of 0.7616 or ~76.2% which was a slightly above the target performance of 75%.

![Final Results](Images/Optimized_Results.png)

### Summary

The deep learning model developed for Alphabet Soup successfully achieved the target accuracy of 75%. The preprocessing steps ensured that the data was suitable for training, and various optimization techniques were applied to improve model performance.

**Recommendations:**
For future efforts, consider exploring other machine learning models such as Random Forests or Gradient Boosting Machines, which can handle different types of data and might provide better performance for this classification problem. These models are often easier to interpret and can provide insights into which features are most important for predicting success.