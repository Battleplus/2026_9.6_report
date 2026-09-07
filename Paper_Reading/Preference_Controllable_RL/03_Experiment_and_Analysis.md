# 3. Experiment and Analysis

## 3.1 Environments

The paper evaluates PCRL in multi-objective reinforcement learning environments.

### Fruit-Tree

Characteristics:

- Discrete environment
- Up to 6 objectives
- Non-strict convex Pareto frontier

This environment tests whether the algorithm can discover diverse Pareto solutions.

### MO-Reacher

Characteristics:

- Robotic control task
- Four conflicting objectives
- Continuous state space

This environment tests preference controllability.

## 3.2 Evaluation Metrics

Two metrics are used:

### Hypervolume (HV)

Measures:

- Pareto frontier coverage
- Diversity of solutions

Higher HV means better exploration.

### Cosine Similarity (CS)

Measures:

- Alignment between user preference and obtained value vector

Higher CS means better preference control.

## 3.3 Main Results

The experiments show:

1. Linear Scalarization finds limited solutions.
2. PCRL can generate different policies for different preferences.
3. PreCo achieves better balance between Pareto optimality and controllability.

## 3.4 Research Understanding

The important contribution is not only improving MORL performance.

The deeper idea is introducing controllability:

Traditional MORL:

```
Objective -> Policy
```

PCRL:

```
Preference + Objective -> Controllable Policy
```

This idea is closely related to preference reinforcement learning and RLHF.
