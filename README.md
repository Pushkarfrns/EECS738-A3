# EECS-738: Neural Network: Says One Neuron To Another (Assignment-3)
This repository contains our submission for EECS-738: Assignment-3.

## Members
- Waqar Ali (2873101)
- Pushkar Singh Negi (2946319)

## Datasets
We have used the following datasets (https://en.wikipedia.org/wiki/List_of_datasets_for_machine-learning_research):
- [default of credit card clients Data Set ](https://www.kaggle.com/uciml/default-of-credit-card-clients-dataset)

## Demonstration
The implementation and documentation of neural network along with their demonstration on the chosen datasets can be seen in the following notebooks:
- [Dataset 1](notebooks/Neural_Network_Implementation.ipynb)

---
<p align="center"><b>Code Summary</b></p>

## Dataset 1: Default of credit card clients
### Columns

- 1. ID
- 2. LIMIT_BAL
- 3. SEX
- 4. EDUCATION
- 5. MARRIAGE
- 6. AGE
- 7. PAY_0
- 8. PAY_2
- 9. PAY_3
- 10. PAY_4
- 11. PAY_5						
- 12. PAY_6
- 13. BILL_AMT1
- 14. BILL_AMT2
- 15. BILL_AMT3
- 16. BILL_AMT4
- 17. BILL_AMT5
- 18. BILL_AMT6
- 19. PAY_AMT1
- 20. PAY_AMT2
- 21. PAY_AMT3
- 22. PAY_AMT4
- 23. PAY_AMT5
- 24. PAY_AMT6
- 25. default.payment.next.month

### Data Analysis
- Loaded the dataset in a dataframe using pandas.
- Checked for null values.
- Removed any unnecessary columns.
- Seperated feature columns and the target column.
- Splitted the data into training set and testing set
- Now our datatset is ready to be passed through Neural Network model.

## Model for Neural Network
Implemented the model by defining Neural_Network_Imp class and repsective functions.

### Function-1:
- Name: __init__
- Purpose: To initiliaze the values for input node, hidden node, output node, weights, learning rate and epochs.
- Input: Faeture array, target array, testing feature ds, testing target ds, learning rate, epochs

### Function-2:
- Name: functionForCalcultingAFSigmoid
- Purpose: Function to calculate the Activation function Sigmoid value.
- Input: self object and input data
- Output: returns the calculated sigmoid.

### Function-3
- Name: functionForCalcultingAFSigmoidDerivative
- Purpose: Function to calculate the derivative of Activation function Sigmoid value.
- Input: self object and input data
- Returns: returns the calculated derivative of sigmoid.

### Function-4
- Name: functionForTrainDataSet
- Purpose: function to train our dataset and build a model.
- Input: self object and  epochs (i.e., Number of times model will be train on the dataset)
- Output: Calculates the % error

### Function-5
- Name: functionForTestingDataSet
- Purpose: function to test our built model and to check the accuracy with the test dataset 
- Input: self object 
- Output: Accuracy of our model with Test data

