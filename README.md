# Udacity_DRL_Projects

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation

### Introduction

For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.


### Solution Description

I trained a deep neural network as an agent the neural network parameters are:

  - 3 hidden layers
  - Used dropout for regularization
  - Leaky ReLU as an activation function for hidden layers
  - Softmax as an activation function for output layer
  - Smooth L1 Loss
  - learing rate: 0.00002
  - discount rate: 0.98
  - replay memory size: 10000
  - Batch size: 64

The model achieved the average score of 10.4. 

I played with learning rate, activation function, dropout rate and number of neurons.
  
