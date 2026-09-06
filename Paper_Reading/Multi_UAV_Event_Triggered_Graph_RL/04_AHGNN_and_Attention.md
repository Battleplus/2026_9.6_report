# AHGNN and Attention

## AHGNN

AHGNN does not directly make task decisions.

Its role is:

> Encode heterogeneous graph information into a decision-oriented embedding representation.

Pipeline:

Original graph

↓

GNN message passing

↓

Node embedding

↓

PPO state input

## Embedding Understanding

Embedding is a vector representation learned by neural networks.

It does not preserve every original detail, but keeps task-related information such as:

- UAV capability
- task compatibility
- neighbor relationships
- execution constraints

## Attention Mechanism

Attention does not directly assign tasks.

It learns the importance of different neighbor information when updating node representations.

The attention parameters are learned during reinforcement learning training through reward feedback.

Training loop:

Reward

↓

Back propagation

↓

Update GNN and Attention parameters

## Key Understanding

Attention answers:

"Which information should be focused on?"

PPO answers:

"Which action should be selected?"
