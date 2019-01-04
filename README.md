# Project: Continuous Control


## Introduction
In this project, the agent is trained to move double-jointed arm to target locations. For each step, the agent can get a reward of 0.1 if the agent's hand reaches the goal location. The agent tries to reach the target for as many time steps as possible.

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/43851024-320ba930-9aff-11e8-8493-ee547c6af349.gif "Trained Agent"
[image2]: https://user-images.githubusercontent.com/10624937/43851646-d899bf20-9b00-11e8-858c-29b5c2c94ccc.png "Crawler"

![Trained Agent][image1]

### Project Details

In the observation space, there are 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. 

The actions space is continuous. Each action is a vector with length of 4, corresponding to torque applicable to two joints. The numbers in the vector of every action should be a between -1 and 1.

### Target of Project

The environment in this project contains 20 identical agents, each with its own copy of the environment. The rewards received by each agent would be sumed up after each episode, then we take the average of the sum of 20 scores and yield the **average score** for each episode.The environment is considered solved when an average score of 20 agents over 100 consecutive episodes is more than +30.



## Getting Started  


1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - **_Twenty (20) Agents_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
   (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.
   

   (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Place the file in the same folder with `continuous_control.ipynb` and unzip (or decompress) the file. 


3. You would need to use the Unity ML-Agents environment in this project. Make sure you have installed [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) and [NumPy](http://www.numpy.org/).

## Instructions


In the `Continuous_Control.ipynb`, when starting the Unity ML-Agetns environment, change the `file_name` parameter to the location of your Unity Environment with `UnityEnvironment(file_name = "your path")`.   

To train the agent, simply run `Continuous_Control.ipynb`. The trained weights of actor and critic networks are stored in files `actor_net.pth` and `critic_net.pth` respectively.



