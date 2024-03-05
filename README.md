# Deep Neural Network Hyperparameter Tuning

For this project, I decided to develop a deep neural network for a multi-class classification problem from [Kaggle's 2024 playground series](https://www.kaggle.com/competitions/playground-series-s4e2). Given the large number of possible architectures and hyperparameters associated with a neural network, I used the Optuna framework to perform Bayesian optimization over a parameter search space. The parameters I explored were:

* Number of hidden layers
* Number of neurons in each hidden layer
* Number of drop out layers and their associated rates
* Activation function for each hidden layer
* Learning rate
* Batch size
* Number of epochs

There is significant overlap in how these variables interact with each other and after a while the Optuna optimization converged in a way that only very small changes were made to learning rates and drop out rates.
