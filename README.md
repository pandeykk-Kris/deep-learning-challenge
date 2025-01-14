## deep-learning-challenge
Alphabet Soup Charity Deep Learning Model
# Purpose of the analysis:
The analysis used real world dataset which contains more than 35k organizations` data, funded by Alphabet Soup in the past. With the help of this data, the aim of the analysis is to create a deep learning neural network model to predict the success/failure of the future funds.
# Results:

# Data Preprocessing
The column named "IS_SUCCESSFUL" was selected as target of this model 
•	During optimization attempts, different feature sets were used to understand their effects on the loss/accuracy.
•	For first optimization attempts "EIN" and "NAME" variables were removed.

# Compiling, Training, optimization and Evaluating the Model
Number of hidden neuron layers and epoch were varied in multiple analyses to determine the effect of model accuracy.

I was able to reach target model performance of 75% by not dropping the NAME column and using three hidden layers of the neural networks. Increasing the number of epochs also showed improved the model accuracy. 


# Three different attempts to optimize the model:

In first attempt, number of epoch was 100.  Accuracy level was 74.60% and the loss was 53.18%. Model was saved as AlphabetSoupCharity.h5 (from notebook named AlphabetSoupCharity)

In second attempt, number of epcoh was increased to 200.  Accuracy level was 73.55 and the loss was 53.33%. 
#
In third attempt (Filename: AlphabetSoupCharity_Optimization-Copy1), I did not drop the NAME column, binned the classification and NAME columns values. Used three hidden neural layers of 30, 20 and 8 respectively.  Accuracy level increased to a value more than 75% to 76.89% and loss of 47.08%. Model was saved as AlphabetSoupCharity_Optimize.h5.
Further increasing the epoch to 200 showed minor improvement of the model (Accuracy 77.02 % and loss 46.71%).

#
Even though not attempted in this exercise, the model can potentially be improved by using other activation functions like Tanh, increasing the number of hidden layers and nodes and using keras tuner library.
