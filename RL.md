Reinforcement Learning:
    Instead of relying on historical data (labeled and unlabeled), reinforcement learning uses 
    rewarded repetition to learn desired behavior on an environment.

    
    GOAL:
        Agent perfom a task on an environment.
    For Example:
        Agent successful in performing some task on an environment
            Win a game of Go (AlphaGo)
            Solve protein folding (AlphaFold)

1. Agent interact with an environment.

Agent:
    How agents interacts with env and rewards and observations back from the env.
    Agent is AI that can observe and interact with the environment.
    Agent can perform actions on the environment and make observations from the environment.
    1. Perforem action
    2. Observe what change in the environment.
    3. Getting observations from the environment

    Agent Example:
        Deep Q Network (DQN) learning agent:
            DQN Agent uses NN as its basis for choosing actions based on the environment.


Agent performs ACTION on the environment.
Agent receives after ACTION agent REWARD or get into some STATE


Environments:
    Agent interact with the environment.
    Agents observation is called state of the world.
    Env can change by the action performed by the agent.
    And it can also change on its own.
    Env can change by factors outside of the control of the agents.
    Agent can observe the env and push the cart left or right i.e perform action on the environment.

STATE vs OBSERVATION:
    STATE:
       A COMPLETE description of the world.  There is NO information about the environment which is hidden from the state. STATE is EVERYTHING that is going on in the environment. No information is HIDDEN OR UNKNOWN. It is difficult to know True entire state of the environment.
       state: When agent is collecting group of observations.
    OBSERVATION:
        Obervation is PARTIAL descritpion of the state, which may OMIT information.
        Usually we get bunch of observation as approxiamation of the state.
States:
    State of an environment.

Observations:
    Observation returned from an environment.

Policy:
    Policy that an agent follows.
    1. What actions were performed.
    2. Observation returned from an environment from performing that action.
    3. Reward returned from performing that action.

    A policy is a RULE used by an agent to decide what actions to take next based on observation and reward received from the environment.
    Given policy it performs action in the env... then based on observation/reward perform another action on the env and cycle continues.

    Agent has policy that considers that look at the policy to determine what actions to perform next.

    Whole time AGENT IS UPDATING policy to MAXIMIZE long term expected REWARD.  Maximize long term REWARD.

2 Types of policies:
Policy is rule used by agent to decide which action to take next.
    Deterministic:
        Directly maps a state to an action.  For any state there is only one possible action to be taken.
        Determines a single course of action.
    Stochastic:
        Family of single probilistic distribution.
        Given a state S you have probability distribution of what action you can take.  Develop prob distribution of what action to take.  This allows us explore alter pathway to explore that goal.


Exploitation Vs Exploration Tradeoff:
    It make sense to explore a lot in the beginning of the game.  Explore less and less as it exploiting or honing its streategy more and more.


Grid World Environment:
    Agent was in the grid.
Tabular Reinforcement Learning:
    QLearning

Rewards:
    Can be -ve or +ve
    Reward is -ve it is awary from  achieveing some goal.
    Reward +ve when it is closer to some overall goal.

Agetn itneract with an env by performing actions
After performing an action it makes an observation and potentially receives a reward.
Based on agent policy it will perform another action.

Discount Factors

Bellman Equation:
    Value of a state = Max value agent can obtain by performing any action.
    V(s) = max(V(s'))


Deterministic Vs Stochastic Processes

Tabular Reinforcement Learning

Q Learning

Classical and Tabular Q Learning



OpenAI Gym:

Keras-Rl2

DQN:
RL + CNN

Learning thru self play not analyzing history.

Policy: Learn using NN.

Value NN:
    Taking in observations/state.
    Pass observations and return values.
    Input layer as same number of inputs as observation.
    Output layer is number of values needed for actual grid.
    When it sees observations it start building these observations are similar to other observations we have seen in the past.
    NN estimate observation to come up with estimated values.
    Key ideas is if two state similar then their values are also similar.

    Compare the past situations that are similar to come up with action to take in the new situation.

    This NN is just producting values not telling us what actions to take.

    Mapping out values to the env given input of observation.

    Taking in observaations from the past and using that to estimate values.

    Value NN: is used to estimate values.

Policy NN:
    Policy decide which action to take.  We will deal with stochastic policy.  We have probability for each neuron in the output layer.

    Each neuron will have probabilist outcome of which action to take.
    Probability for each state.
    Policy for similar state.


We will build 2 linked but separate NN.  Link these by assigning them same weights.

Exploitation and Exploration Tradeoff









