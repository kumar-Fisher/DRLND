![image](/p1_navigation/banana.gif)
### Project Overview
________________________________________
    For this project, you will train an agent to navigate (and collect bananas!) in a large, square world.
    A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.
    The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:
    •	0 - move forward.
    •	1 - move backward.
    •	2 - turn left.
    •	3 - turn right.
    The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.



### Step 1: Install Dependencies

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

### Step 2: Clone the repo
    Clone this repo using git clone https://github.com/kumar-Fisher/DRLND.git.

### How to run the code in the repository
1.  Setup Python Environment

Please follow the instruction to [setup Python environment](https://github.com/udacity/deep-reinforcement-learning#dependencies) from the original course GitHub repository.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file. 

### Instructions to run Navigation.ipynb
1.  Open the file Navigation.ipynb in jupyter notebook
2.  Run the each cell of the file follow the instruction in the file
3.  This will tarin your model.
4.  Once the model is trained it will be saved in saved_model.pth file
5.  Run the environment with trained model you will see the score is higher

