# 2. Method

## 2.1 Overview

The proposed framework is Preference Controllable Reinforcement Learning (PCRL).

The main idea:

> Train one preference-conditioned policy that receives user preference as input and outputs a policy located at the corresponding region of the Pareto frontier.

Framework:

```
Preference p
      |
      v
Preference-conditioned Policy π(a|s,p)
      |
      v
Multi-objective Value Vector vπ
      |
      v
MOO gradient optimization
      |
      v
Pareto optimal preference-controlled policy
```

## 2.2 Preference Conditioned Policy

Instead of training independent policies for different preferences, PCRL learns:

$$
\pi(a|s,p)
$$

where:

- s: environment state
- a: action
- p: user preference vector

Different preference vectors lead to different behaviors.

## 2.3 PreCo Update

The core contribution is Preference Control (PreCo).

The update combines:

1. Objective gradients
2. Preference similarity gradient

The optimization direction is:

$$
d^*=\nabla^Tv^\pi w^*+\lambda\nabla\Psi(p,v^\pi)
$$

where:

- w*: gradient balancing coefficient
- Ψ: preference similarity function
- λ: preference control strength

Unlike conventional MOO methods, PreCo does not only search for Pareto improvement, but also pushes the solution toward the desired preference.

## 2.4 Intuition

Traditional MORL:

"Find any good Pareto solution"

PCRL:

"Find the Pareto solution that matches this user's preference"
