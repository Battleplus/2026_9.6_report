# GPPO Understanding Notes

## 1. Why GPPO?

Traditional PPO receives state vectors directly:

```
State -> PPO -> Action
```

However, multi-UAV task allocation contains complex relationships:

- UAV-task capability matching
- Task-task dependency

Therefore, graph representation is introduced before PPO.

```
Heterogeneous Graph
        |
        v
GNN Encoding
        |
        v
Embedding
        |
        v
PPO Decision
```

---

## 2. Actor-Critic Structure

### Actor

Actor decides actions:

```
Which UAV executes which task?
```

It learns the policy:

pi(a|s)


### Critic

Critic estimates future value:

V(s)

It evaluates how valuable the current state is under the current policy.

---

## 3. Parameter Updates

During training:

Reward feedback updates:

- PPO Actor parameters
- PPO Critic parameters
- GNN parameters
- Attention parameters

The final deployment usually uses fixed parameters for inference.

---

## 4. Reward

The reward is related to task completion efficiency.

A key metric is Makespan:

The total time required for all tasks to finish.

The objective is reducing overall completion time.
