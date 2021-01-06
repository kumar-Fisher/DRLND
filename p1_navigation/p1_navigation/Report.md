# Algorithm implementation details

### Q-Network Class
Q-Network class implemnts the neural network which consists of two fully connected (FC) hidden layers.
First FC late has 1024 nodes connected to input layer and second FC layer has 64 nodes connected to output layer. 
Both of the Fully Connected layers have RELU activation function. The input has 37 nodes (environment state ) 
and the output has 4 nodes (action space).The two hidden layers and the RELU activation function are chosen to achieve non-linearity. Whereas, 
the high number of nodes are selected so the model can have better learning capability. 

### Replay Buffer
Replay Buffer is used to stores tuples of state, action, reward, next state and done flag of an experience once the replay 
buffer size is more then the Batch size then the nural network is trained. To overcome the problem of co-relation sampling of the experience are
sampled from the replay buffer randomly.

### Agent

Agents interacts with the environment and and get experince and update the replay buffer.Once the replay buffer is grater then the batch size
then the nural network trained.


### Training

Discount factor (gamma) for training is set high at 0.99 and the exploration value epsilon start at high value (1.0) but then gradually going 
down to 0.01. The target average score of 13 or higher in 100 episodes window was achieved in 472 episodes. The learning progress is shown below.

![Learning Scores](./image/score_vs_episode.PNG)

### Agent Performance

Initially, when the exploration value was 0.01, the agent was trapped state-action loop. 
After makeing it higher at 0.1, the trained agent performd much batter and easily achieved score of 13.

### Future Work
Double DQN method can be used for faster and more stable learning.
Prioritized Experience Buffer can be used.
As currently the Q-Network uses massive first fully connected node 1024 
just to make sure that agent has the capability to perform well this can be reduced to 256