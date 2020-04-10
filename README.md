# Udacity Deep Reinforcement Learning Project 2 Continuous Control

## Train a Set of Robotic Arms

![Unity ML-Agents Reacher Environment](https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif)


## Background

This repository of DeepRL source code is the work of the 2nd Project in this Nanodegree at the end of Part2, Policy-Based Methods including DDPG (Deep Deterministic Policy Gradient). The project goal is to train a policy-based agent which controls a robot arm to touch and follow a ball which i swinging provided by the simulated environment which is created by using Unity ML-Agents


## Environment

In this environment, a double-joint arm can move to a target location. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of the agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

The environment contains 20 identical agents, each with its own copy of the environment


## Solving Criterias

Take the average of each agents (potentially different) 20 scores for each episode.
The environment is considered solved, when the average (over 100 consecutive episodes) of those average scores is at least +30


## Getting Started 

1. Check [this nanodegree's prerequisite](https://github.com/udacity/deep-reinforcement-learning/#dependencies), and follow the instructions.

2. Clone this repository, change directory, and activate *drlnd* environment.
``` bash
git clone https://github.com/baerwind/p2-Continuous
chdir p2-Continuous
source activate drlnd
```

3. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

  - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
  - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
  - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
  - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

4. Place the file in the DRLND GitHub repository, in the `./bin/` folder, and unzip (or decompress) the file. 

5. Follow the instructions in Continuous_Control.ipynb to get started with training your own agent!