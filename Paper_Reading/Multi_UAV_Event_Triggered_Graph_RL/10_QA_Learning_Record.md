# Learning Q&A Record

## Q1: Why does PPO need GNN?

PPO can learn policies but does not explicitly understand graph relationships. GNN converts relational information into embeddings.

## Q2: Does embedding lose information?

Yes, but it keeps task-related high-level information rather than all raw details.

## Q3: Why can Attention be learned?

Attention parameters are optimized together with reinforcement learning. Reward feedback updates attention weights indirectly through back propagation.

## Q4: Why not let PPO learn importance directly?

Without attention, PPO must simultaneously learn representation and decision making. Attention separates information aggregation from action selection.

## Q5: Actor and Critic

Actor:
selects actions.

Critic:
estimates future cumulative value of the current state.

## Q6: Training vs Deployment

Training:
update GNN, Attention, Actor and Critic parameters.

Deployment:
usually keep parameters fixed and perform inference.

## Final Understanding

GNN understands relationships.
Attention selects useful information.
PPO makes decisions.
Event Trigger determines when replanning is needed.
