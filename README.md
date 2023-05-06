# Connect-Four-Reinforcement-Learning

Project as part of Optimization II Coursework

# Description

Connect Four PopOut Reinforcement Learning

This project implements the Policy Gradient method in Reinforcement Learning to train a neural network to play the game of Connect Four PopOut.

The Policy Gradient approach involves training a classification model to output the probability of each action being the best, without explicitly optimizing the value function. This method was chosen as it is more suitable for this project, which involves a complex and high-dimensional state space.

The game functions, such as update_board, check_for_win, display_board, get_legal_move, play1random, and play1opp, were implemented to set up the game and simulate gameplay between the player and the AI.

The create_model function creates a neural network using the Keras API, which is trained with our policy gradient to play the game. The input layer has the shape of the height and width of the game board, followed by two 1D Convolutional layers using a ReLU Activation function with 16 and 8 filters and a kernel size of 2, respectively. Two fully connected hidden layers using a ReLU Activation function with 32 and 64 units are added, and the output from the previous layer is flattened to a 1D array. Another dense layer using a ReLU Activation function is added, and the output layer uses a Softmax Activation function to produce a probability distribution over the possible actions.

This project provides a useful example of how to apply Reinforcement Learning to a complex game like Connect Four PopOut, and the code can be used as a reference to build other AI agents for similar games.
