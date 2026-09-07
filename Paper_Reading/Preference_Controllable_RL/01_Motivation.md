# 1. Motivation

## 1.1 Background

Many real-world reinforcement learning tasks require optimizing multiple objectives simultaneously.

Examples:

- Robot control: speed vs safety
- Autonomous driving: efficiency vs risk
- Game agents: reward maximization vs user preference

Traditional RL usually assumes a single scalar reward, but practical problems often contain conflicting objectives.

## 1.2 Problem of Existing MORL

Multi-Objective Reinforcement Learning (MORL) attempts to learn policies under multiple objectives.

A common approach is Linear Scalarization (LS):

$$
max_\pi p^T v^\pi
$$

where preference vector p represents the importance of each objective.

However, LS has two major limitations:

1. It can only discover a subset of Pareto optimal solutions.
2. The obtained solution may not match the user's desired preference.

Therefore, although the policy receives preference information, it may not be controllable by preference.

## 1.3 Key Question

The paper focuses on:

> How can we train a single RL agent that can generate different optimal behaviors according to different user preferences?

The authors propose Preference Controllable Reinforcement Learning (PCRL).

The preference vector is directly used as a condition of the policy:

$$
\pi(a|s,p)
$$

allowing one agent to produce different trade-offs on the Pareto frontier.
