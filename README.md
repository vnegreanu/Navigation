# Project : Navigation

## Description 
For this project, we train an agent to navigate in a large square world
collecting yellow and blue bannanas differentiating by this positive from
negative events using DQN algorithm

![Trained Agent](images/TrainedAgent.gif)

## Problem statement 
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided 
for collecting a blue banana. Thus, the goal of the agent is to collect 
as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions, and contains the agent's velocity, along
with ray-based perception of objects around the agent's forward
direction. Given this information, the agent has to learn how to best select 
actions. 
Four discrete actions are available, corresponding to: 
- `0` - move forward
- `1` - move backward
- `2` - turn left
- `3` - turn right
The task is episodic, and in order to solve the environment, the 
agent must get an average score of +13 over 100 consecutive episodes.

## Files
- `Navigation.ipynb`: Notebook used to control and train the agent 
- `DQN/dqn_model.py`: DQN implementation used to control and train the agent for experimentation
- `DQN/dqn_agent.py`: Agent class that interacts with and learns from the environment 
- `DQN/replay_buffer.py`: Internal class used to map states to action values
- `saved_data/model.pth`: Saved model weigths
- `README.md`: README file with project description
- `install_requirements.txt`: File with python packages install dependencies
- `report.pdf`: Technical report on the project. Algorithm choise, design decission, future improvements,etc... 

## Dependencies
To be able to run this code, you will need an environment with Python 3 and 
the dependencies are listed in the `install_requirements.txt` file so that you can install them
using the following command: 
```
pip install install_requirements.txt
``` 

Furthermore, you need to download the environment from one of the links below. You need only to select
the environment that matches your operating system:
- Linux : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
- MAC OSX : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
- Windows : [link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

## Running
Run the cells in the notebook `Navigation.ipynb` to train an agent that solves our required
task of collecting bananas.

