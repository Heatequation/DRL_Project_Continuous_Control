# Report

### Learning Algorithm
The agent learns through the Deep Deterministic Policy Gradients (DDPG) algorithm. It is amended to allow for distributed gathering of experience. The implementation of the DDPG algorithm is based on the research paper [
Continuous control with deep reinforcement learning](https://arxiv.org/abs/1509.02971): 
  
The model architecture is a deep neural network with one hidden layer. Input and hidden layer use ReLu activation.  
  
The following hyperparameters are used:
* replay buffer size: BUFFER_SIZE = int(1e5)
* minibatch size: BATCH_SIZE = 64
* discount factor: GAMMA = 0.99
* soft update of target parameters: TAU = 1e-3
* learning rate: LR = 1e-4
* how often to update the network: UPDATE_EVERY = 4

### Training Results
(Update) The trained agent solved the environment in 129 episodes. The following plot shows the rewards per episode:
![reward plot](https://github.com/Heatequation/DRL_Project_Navigation/blob/master/reward_episodes.png)


### Ideas for Future Work
More advanced techniques could be employed. For example:
* Trying a different fundamental algorithm like (PPO, ...)
* Trying a different fundamental algorithm like (PPO, ...)
* Trying a different fundamental algorithm like (PPO, ...)
* Improving the DDPG implementation: Parameter Noise instead of Action Noise (Open AI Gym's article)
* Improving the DDPG implementation: Parameter Noise instead of Action Noise (Open AI Gym's article)
* Improving the DDPG implementation: Parameter Noise instead of Action Noise (Open AI Gym's article)
