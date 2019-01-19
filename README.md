# DRL_Continuous_Control

### Introduction
For this project, the Reacer environement is used. The agent is represented by 20 copies of a double-jointed arm. The aim is to learn for every arm how to keep its hand in a moving goal location.
This is a project to demonstrate the application of deep reinforcement learning. Specifically the DDPG algorithm and distributed training.

The training was executed in the iPython notebook. The agent is defined in file ddpg_agent.py and the aritficial neural networks used to make the agent learn is in file model.py.

The environment in which each individual double-jointed arm acts can be descriped the following way:
* state space: There are 33 dimensions corresponding to position, rotation, velocity, and angular velocities of the arm
* action space: The action space is continuous and consists of 4 dimensions corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.
* reward: A reward of +0.1 is provided for each step that the hand is in the goal location.

The environment is considered solved, when the average over 100 episodes of the agent's score is at least +30. Where the agent's score from episode i is defined as: the average of the scores of all 20 arms attained in episode i.

### Getting Started

1. Download the Reacher environment from one of the links below depending on your operating system.
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

2. Unzip file in this repository's root folder.

### Instructions

Setup a python environment as described [here](https://github.com/udacity/deep-reinforcement-learning#dependencies).

Then train the agent by following the instructions in `Continuous_Control.ipynb`. 
