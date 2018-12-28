[//]: # (Image References)

[image1]: https://s3.amazonaws.com/video.udacity-data.com/topher/2018/May/5af7955a_tennis/tennis.png "Trained Agent"

# Project 2: Collaboration and Competition

### Introduction

For this project, I trained two agents to control a racket to bounce a ball over a net.

![Trained Agent][image1]

If an agent hits the ball over the net, it receives a reward of +0.1. If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01. Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation. Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping.

The task is episodic, and in order to solve the environment, the agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents).

### Files

- Collaboration and Competition.ipynb - code for agent
- README.md - this file
- Report.pdf - a report on the algorithm used to train the agents and its performance
- requirements.txt - dependencies required by agent's code
- checkpoint_actor_0.pth - actor model weights for agent 1 that successfully solved the control task
- checkpoint_critic_0.pth - critic model weights for agent 1 that successfully solved the control task
- checkpoint_actor_1.pth - actor model weights for agent 2 that successfully solved the control task
- checkpoint_critic_1.pth - critic model weights for agent 2 that successfully solved the control task

### Getting Started

NOTE: This code requires Python 3.6

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the root directory and unzip (or decompress) the file. 
3. Open Collaboration and Competition.ipynb and replace `<path to Tennis environment just unzipped/uncompressed>` (in 2. Fetch the environment) with the path to the file from Step 2 above.

### Training the Agents

The code is contained in an interactive notebook, Collaboration and Competition.ipynb. So all you need to do is run each code cell, one after the other.