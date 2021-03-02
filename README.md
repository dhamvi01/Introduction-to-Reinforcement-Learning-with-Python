# Introduction-to-Reinforcement-Learning-with-Python

## What is Reinforcement Learning?
Reinforcement Learning (RL) is a branch of machine learning concerned with actors, or agents, taking actions is some kind of environment in order to maximize some type of reward that they collect along the way.

In supervised learning, for example, each decision taken by the model is independent, and doesn't affect what we see in the future.

In reinforcement learning, instead, we are interested in a long term strategy for our agent, which might include sub-optimal decisions at intermediate steps, and a trade-off between exploration (of unknown paths), and exploitation of what we already know about the environment.

## Terminology
We will now take a look at the main concepts and terminology of Reinforcement Learning.

  - Agent
    A system that is embedded in an environment, and takes actions to change the state of the environment. Examples include mobile robots, software agents, or industrial controllers.

  - Environment
    The external system that the agent can "perceive" and act on.Environments in RL are defined as Markov Decision Processes (MDPs). A MDP is a tuple.
    A lot of real-world scenarios can be represented as Markov Decision Processes, from a simple chess board to a much more complex video game.

    In a chess environment, the states are all the possible configurations of the board (there are a lot). The actions refer to moving the pieces, surrendering, etc.

    The rewards are based on whether we win or lose the game, so that winning actions have higher return than losing ones.

Reward Function
A lot of research goes into designing a good reward function and overcoming the problem of sparse rewards, when the often sparse nature of rewards in the environment doesn't allow the agent to learn properly from it.

Value Function
The value function is probably the most important piece of information we can hold about a RL problem.
Formally, the value function is the expected return starting from state s. In practice, the value function tells us how good it is for the agent to be in a certain state. The higher the value of a state, the higher the amount of reward we can expect:

Policy
The policy defines the behaviour of our agent in the MDP.
Formally, policies are distributions over actions given states. A policy maps states to the probability of taking each action from that state:
The ultimate goal of RL is to find an optimal (or a good enough) policy for our agent. In the video game example, you can think of the policy as the strategy that the player follows, i.e, the actions the player takes when presented with certain scenarios.


