# 02 World Model Background

## Model-free RL
Directly learns policy or value function through environment interaction.

## Model-based RL
Learns environment dynamics and uses the model to improve decision making.

## World Model
A world model learns how the environment evolves, allowing agents to generate imagined trajectories for policy learning.

## Difference Between World Model and Critic

World Model:
Predicts environment changes.
Example: If an action is taken, what may happen next?

Critic:
Evaluates the value of a state or action.
Example: How good is this action in the long term?

## Why Need World Model?
Real environment interaction is expensive. By learning a model, agents can train policies using imagined future trajectories.

## Key Point of EAWM
Traditional world models focus on observation prediction. EAWM adds event prediction to learn more meaningful dynamic representations.
