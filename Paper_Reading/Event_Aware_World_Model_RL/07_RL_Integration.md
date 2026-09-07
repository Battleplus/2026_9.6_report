# 07 RL Integration

## How World Model Connects With RL

World Model:
Predicts possible future environment changes.

Actor:
Learns which action to choose.

Critic:
Evaluates the value of states or actions.

## Training Process

1. Collect real environment data.
2. Train world model.
3. Generate imagined trajectories.
4. Use Actor-Critic learning on imagined experience.

## Important Difference

World Model predicts environment dynamics.
Critic predicts expected return.

They solve different problems.

## Test

If World Model prediction is wrong, why can it influence policy learning?
