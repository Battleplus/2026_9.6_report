# Experiment Analysis

## Main Verification Goals

The experiments should verify:

1. Whether graph representation improves task allocation.
2. Whether attention improves information selection.
3. Whether event-triggering reduces communication cost.
4. Whether the method adapts to dynamic environments.

## Common Metrics

### Makespan

Overall task completion time.

Lower is better.

### Reward

Reflects optimization during reinforcement learning.

### Communication Cost

Measures the benefit of event-triggered updates.

### Computation Cost

Evaluates practical deployment feasibility.

## Ablation Logic

Remove GNN:
- verify graph modeling contribution.

Remove Attention:
- verify importance weighting contribution.

Remove Event Trigger:
- verify communication efficiency contribution.
