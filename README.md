# Default Prediction Using MLP

## Overview
This project implements a Multi-Layer Perceptron (MLP) using TensorFlow to predict defaults on credit card payments. The dataset used is the "Default of Credit Card Clients" dataset, which contains financial information on clients and whether they defaulted on their payments. The objective is to build a predictive model that can assist financial institutions in assessing credit risk.

## Dataset
https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients<br>
The dataset can be found here.<br>

## Model Architecture
The MLP consists of the following layers:
- **Input Layer:** Takes in 23 numerical features from the dataset.<br>
- **Hidden Layers:**<br>
  - First hidden layer with 64 neurons and ReLU activation.<br>
  - Second hidden layer with 32 neurons and ReLU activation.<br>
- **Output Layer:**<br>
  - A single neuron with a sigmoid activation function for binary classification (default vs. no default).<br>

## What the Code Accomplishes
This code experiemnts with what is the best optimiser for the model being trained on this dataset. Although the resulting graphs in the experement has a confusing output.<br>
![TRAINING LOSS](/Users/Ben/Documents/01 LSE/ST456 - Deep Learning /Week 2/Defualting/TRAINING LOSS.png)<br>
![VALIDATION LOSS](/Users/Ben/Documents/01 LSE/ST456 - Deep Learning /Week 2/Defualting/VALIDATION LOSS.png)<br>
I cannot understand why when testing that Adam and RMSprop seem to have an increasing loss. 

## Future Improvements
- Add more layers to the model and change the number of nodes in the hidden layers.
- Apply a different method of regularization (Dropout, Early Stopping)



