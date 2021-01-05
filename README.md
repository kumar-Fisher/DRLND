Project Overview
________________________________________
For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:
•	0 - move forward.
•	1 - move backward.
•	2 - turn left.
•	3 - turn right.
The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.



Step 1: Install Dependencies

Create an anaconda  environment that contains all the required dependencies to run the project.
Mac:

conda create --name drlnd_continuous_control python=3.6

source activate drlnd_continuous_control

conda install -y python.app

conda install -y pytorch -c pytorch

pip install torchsummary unityagents

Windows:

conda create --name drlnd_continuous_control python=3.6

activate drlnd_continuous_control

conda install -y pytorch -c pytorch

pip install torchsummary unityagents
Step 1: Clone the repo

Clone this repo using git clone https://github.com/kumar-Fisher/DRLND.git.