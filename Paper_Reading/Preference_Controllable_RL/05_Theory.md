# Theoretical Analysis

## Pareto Stationary Convergence

The paper proves that PreCo converges to Pareto stationary points under several assumptions:

- Objective smoothness
- Bounded stochastic gradient variance
- Lipschitz continuity

## Main Idea

The algorithm searches for a direction where:

- all objectives can improve together
- preference similarity is increased

When no common improving direction exists, the policy reaches Pareto stationary state.

## Preference Controllability

The paper further analyzes whether the learned policy value vector approaches the requested preference direction.

Theoretical results show that the similarity gradient can converge, allowing preference-specific solutions.

## Understanding

The theory provides a guarantee that optimization does not only find Pareto optimal solutions but also makes them controllable according to user requirements.
