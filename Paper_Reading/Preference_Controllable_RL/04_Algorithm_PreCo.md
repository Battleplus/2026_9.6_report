# PreCo Algorithm Analysis

## 1. Core Problem

Traditional MORL methods often optimize a weighted reward:

$$J(\pi)=p^Tv^\pi$$

where p represents objective preference.

However, Linear Scalarization cannot cover the complete Pareto front and may fail to achieve the desired preference point.

## 2. PCRL Framework

PCRL introduces preference p as an input condition:

$$\pi(a|s,p)$$

The same policy network can generate different behaviors according to different user preferences.

## 3. PreCo Update

PreCo combines two gradients:

1. Objective gradients
- Improve multiple objectives
- Maintain Pareto optimality

2. Similarity gradient
- Move the obtained value vector toward the preference direction

The final update direction is obtained by solving a minimum norm optimization problem.

## 4. Intuition

Normal MORL asks:

"Can I find good solutions?"

PCRL asks:

"Can I find the solution that matches this specific preference?"

PreCo adds controllability on top of Pareto optimization.

## 5. Connection

This idea is similar to preference optimization in RLHF:

human preference -> optimization target -> controllable policy

PCRL extends this idea from single reward alignment to multiple conflicting objectives.
