# Module 19 | Neural Network Analysis

## Overview

The purpose of this project is to design a Neural Network Model to make the decision about which companies should receive donations from a company named "Alphabet Soup"

## Results

### Data Preprocessing

Inspecting the data we established the target variable as *"IS_SUCCESSFUL"* column. Then we removed the *"EIN*" and *"NAME"* columns as they did not offer any relevant data that could help the model perform better.

### Compiling, Training, and Evaluating the Model

For the **first attempt** at compiling a neuron network which consisted of 8 neurons in the first layer and 6 in the second layer; Both layers had **relu activation** functions and the output layer had a sigmoid activation function. I started with these parameters as relu does better with nonlinear data, and two layers which allow for a second layer to reweight the inputs from the first layer. The we removed the *"SPECIAL_CONSIDERATIONS"* column to avoid confusing the model. We lowered the threshold for the classification column so that there were more unique values from that column and added a third layer with 6 neurons apart of it. This were the results:
![ASC_Ov1_scores](https://github.com/davescudero/Neural_Network_Charity_Analysis/blob/main/Resources/ASC_Ov1_scores.png)

In the next attempts, we decided to revert back the threshold for the classification column, then we changed the activation function for the three layers to tanh. We changed the neurons to 12 in the first layer and 8 in the second layer. We decided to increase the parameters passed from the first layer to the second layer from 54 to 104. This were the results:.
 did this to see if it would perform better than the relu function.
![ASC_Ov2_scores](https://github.com/davescudero/Neural_Network_Charity_Analysis/blob/main/Resources/ASC_Ov2.png)

## Summary

Finally after all the attempts to train the model, we were not able to perform an accuracy up to 75%, even though we added more "layers" to the model.
We suggest to perform a different type of analysis like Random Forest, an to get to know better about activation function to choose according to data.
