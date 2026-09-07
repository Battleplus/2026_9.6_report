# Relation to World Model and GPPO

## 1. Connection with World Model

World Model focuses on learning a predictive model of environment dynamics. It answers:

> What will happen after taking an action?

Preference Controllable RL focuses on:

> Which future outcome should the agent prefer when objectives conflict?

Therefore, World Model provides prediction ability, while PCRL provides preference-based decision control.

A possible combination:

1. World Model predicts multiple imagined trajectories.
2. Each trajectory is evaluated by multiple objectives.
3. Preference-conditioned policy selects the trajectory aligned with user preference.

## 2. Connection with Preference RL

PCRL is closely related to preference-based reinforcement learning.

Traditional RLHF learns from human preference signals to optimize a scalar reward. PCRL instead keeps multiple objectives explicitly and learns controllable trade-offs.

Advantages:

- avoids collapsing multiple objectives into one reward
- allows users to change preference dynamically
- provides Pareto-optimal solutions

## 3. Connection with GPPO

GPPO usually improves policy optimization through better gradient estimation or policy update strategies.

PCRL provides another perspective:

Instead of asking:

"How to optimize one reward better?"

PCRL asks:

"How to optimize multiple conflicting goals while allowing controllable preference changes?"

Possible combination:

GPPO + PCRL:

- GPPO improves optimization stability
- PCRL provides preference controllability
- World Model provides imagined rollouts

This combination could form a preference-controlled model-based agent framework.

## 4. Research Inspiration

A future direction:

Event-Aware World Model + Preference Controllable RL

Pipeline:

Observation -> Event extraction -> World Model prediction -> Multi-objective evaluation -> Preference-conditioned policy -> Action

This could enable agents that not only predict future events but also choose futures according to different user preferences.
