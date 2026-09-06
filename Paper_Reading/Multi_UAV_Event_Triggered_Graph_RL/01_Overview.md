# Multi-UAV Dynamic Task Assignment Based on Event-Triggered Graph Reinforcement Learning Under Weak Communication

## 1. Problem Background

The paper focuses on dynamic multi-UAV task assignment under weak communication environments.

Main challenges:

- UAVs have heterogeneous capabilities.
- Tasks contain complex dependencies.
- The environment changes dynamically.
- Communication resources are limited.

The goal is to achieve efficient task allocation while maintaining adaptability.

---

## 2. Overall Framework

```
Dynamic Environment
        |
        v
UAV State + Task State
        |
        v
Heterogeneous Graph
        |
        v
AHGNN
        |
        v
Attention Enhanced Representation
        |
        v
Embedding State
        |
        v
GPPO
        |
        v
UAV-Task Assignment
```

---

## 3. Core Idea

The paper combines:

- Heterogeneous graph representation
- Graph neural network encoding
- Attention mechanism
- PPO reinforcement learning
- Event-triggered communication

The key idea is:

Use graph learning to understand relationships, then use PPO to make dynamic allocation decisions.
