# DDPG report



## Introduction

This repository is the solution for the second assignment in the Udacity Deep Reinforcement Learning Nanodegree. The goal was to train an agent using policy based methods (in this case, using a DDPG) that was able to sucessfully solve the "Reacher" environment made by Unity ML Agent and collect enough rewards, represented by grasping a certain region, in order to achieve a score above a certain threshold. We'll be introducing the Project details.

## Project details

The following iterals contains the description of the environment

a. State

In this case, the state consists of one single agent, who has 33 variables in the observation space, which describe things such as position, velocity, rotation and angular velocities of the arm.

b. Action spaces

Every action performed consists of a vector of four numbers, corresponding to torque applicable to two joints. Every number in the action vector has a range between -1 and 1. 

It is important to note that the agent doesn't act directly with the environment. A so called "brain" controls the actions within the environment and collects the information from the state.

c. Solved 

The task is episodic (it is not eternal, it ends after a while), and the environment is considered solved when the agent achieves an average score of +30 over a window of 100 consecutive episodes. 


## Getting started

a. Unity ML Agents:

First you must install the Unity toolkit. You'll find the instruction in this link, please don't dispair, this is probably the hardest step: <href>https://github.com/udacity/deep-reinforcement-learning#dependencies
	
b. Install
	
After you have downloaded the toolkit please install it and then download the reacher environment you can find it in the following link:  https://github.com/udacity/deep-reinforcement-learning/tree/master/p2_continuous-control.
	
c. Play

Have fun! The implentation of the DQN has two files files: AC_model.py, and Agent_Continuous_Control.ipynb
* AC_model.py
-This file contains the implementation of both the actor and the critic class, which the other model uses to run the network. Both of them describe the DNN (Deep Neural Network) used by both the actor and the critic process
* Agent_Continuous_Control.ipynb
-This jupyter notebook uses the model file and, after downloading the dependencies (if needed) it starts playing with the environment. After that, the DDPG model is defined and then the DDPG process is executed.

## Instructions

Just as highlighted above if you want to train the model from scratch run the navigation jupyter notebook. Otherwise you can use the pretrained checkpoint (denoted as ..._final for both actor and critic) provided in the repository.   


 

