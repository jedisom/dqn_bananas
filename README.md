[//]: # (Image References)
[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Going Bananas!

### Project Details

In this project a deep neural network reinforcement learning agent learns how to navigate (and collect bananas!) in a large, square world.  The square world environment is provided by Unity's open source Machine Learning Agents (ML-Agents) plugin that enables games and simulations to serve as environments for training intelligent agents.   

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the trained agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space provided by the Unity environment has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the agent must get an average score of +13 over 100 consecutive episodes.  The baseline performance for this task reaches an average score of +13 after 1800 episodes.

### Getting Started
To set up your computer to run the python code in this repository, follow the instructions below.

1. Install/Setup Python 3.6+.   See the instructions for how to do this for your operating system on the official [www.python.org](www.python.org) website.

2. [Install pip for python](https://pip.pypa.io/en/stable/installing/)

3. Install dependent python packages
    - numpy (e.g. `pip install numpy`)
    - matplotlib (see [installation instructions](https://matplotlib.org/faq/installing_faq.html))
    - pytorch: Select the correct options in the "Getting Started" section of the [pytorch main page](https://pytorch.org/), then run the command created in the "Run this command:" section of that webpage.
    - jupyter notebook: (e.g. `pip install jupyter`).  If simple pip install doesn't work see jupyter's [official documentation](http://jupyter.org/install)
    
4. Follow the instructions in [this repository](https://github.com/openai/gym) to perform a minimal install of OpenAI gym.

    - Next, install the classic control environment group by following the instructions [here](https://github.com/openai/gym#classic-control).

5. Clone this GitHub repository that contains my solution to the problem.  
    - Navigate to the folder where you want to install the repository (e.g. cd C:/bananas/)

    - `git clone https://github.com/jedisom/dqn_bananas.git`

        `cd deep-reinforcement-learning/python`

        `pip install .`

6. Create an IPython kernel for the drlnd environment.

    e.g. `python -m ipykernel install --user --name drlnd --display-name "drlnd"`

    Before running code in a notebook, change the kernel to match the drlnd environment by using the drop-down Kernel menu.
Kernel

### Running the Agent

Start by opening a Jupyter Notebook
1. Open a command prompt/terminal and type `jupyter notebook`.  If that doesn't work, return to step 3 of "Getting Started" above to successfully install jupyter notebook.
2. Navigate to the dqn_bananas project folder you cloned from GitHub
3. Open the `Navigation.ipynb` notebook
4. Read instructions in the notebook and execute each line of code by pressing `SHIFT + ENTER`