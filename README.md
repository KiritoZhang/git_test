
### Project Details

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

Set-up: Two-player game where agents control rackets to hit a ball over the net.

Goal: The agents must hit the ball so that the opponent cannot hit a valid return.

Agent Reward Function (independent):
- +1.0 To the agent that wins the point. An agent wins a point by preventing the opponent from hitting a valid return.
- -1.0 To the agent who loses the point.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

Behavior Parameters:
- Vector Observation space: 9 variables corresponding to position, velocity and orientation of ball and racket.
- Vector Action space: (Continuous) Size of 3, corresponding to movement toward net or away from net, jumping and rotation.
- Visual Observations: None

Float Properties: 
- gravity: Magnitude of gravity
- Default: 9.81
- Recommended Minimum: 6
- Recommended Maximum: 20
- scale: Specifies the scale of the ball in the 3 dimensions (equal across the three dimensions)
- Default: .5
- Recommended Minimum: 0.2
- Recommended Maximum: 5


In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

The task is episodic, and in order to solve the environment, your agents must get an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents). Specifically,

- After each episode, we add up the rewards that each agent received (without discounting), to get a score for each agent. This yields 2 (potentially different) scores. We then take the maximum of these 2 scores.
- This yields a single **score** for each episode.

The environment is considered solved, when the average (over 100 episodes) of those **scores** is at least +0.5.

### Getting Started

1. First download the appropriate environment from the Udacity link.
    - Windows (64-bit): https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip

2. Then place the file in the "p3_collab-compet /" folder in the DRLND GitHub repository and then unzip (or unzip) the file.

3. Finally, you need to install some libraries via pip.
    - unityagents
    - collections
    - matplotlib
    - numpy
    - random
    - copy
    - os
    - torch

### Instructions

I have solved the environmental problem in `Tennis.ipynb`, just need to run the code in order.
