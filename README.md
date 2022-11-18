# Project 2: Continuous Control

## Introduction
This project is one of the assignments in [Deep Reinforcement Learning Nanodegree Program](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893), offered by Udacity.  

For this project, we're attempting to solve the the Reacher environment.
![](./img/environment_illustration.gif)


## Understanding the environment


In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The project environment provided by Udacity is similar to, but not identical to the Reacher environment on the [Unity ML-Agents GitHub page](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#reacher).  



#### Solving the environment

We were required to solve 1 out of the 2 versions of environment provided and **Version 2: Twenty (20) Agents** was selected for this repository.

* **Version 1: One (1) Agent**  
The task is episodic, and in order to solve the environment, the agent must get an **average score of +30 over 100 consecutive episodes**.

* **Version 2: Twenty (20) Agents**  
The barrier for solving the second version of the environment is slightly different, to take into account the presence of many agents. In particular, your agents must get an average score of +30 (over 100 consecutive episodes, and over all agents). Specifically,

After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 20 (potentially different) scores. We then take the average of these 20 scores.
This yields an average score for each episode (where the average is over all 20 agents).


## Included in this repository

* The code used to create and train the Agent
  * Continuous_Control.ipynb
* The trained model
  * checkpoint.pt
* A Report.md file describing the development process and ideas for future work
* This README.md file

## Getting started
The project was done solely in the Udacity workspace and the only preparatory step needed to start the project was by running the command below to install the needed packages:

```
!pip -q install ./python
```


</br>
