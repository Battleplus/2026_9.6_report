# Heterogeneous Graph Modeling

## Motivation

Traditional PPO receives vector states and cannot explicitly represent relationships between UAVs and tasks.

The paper models the environment as a heterogeneous graph.

## Node Types

### UAV Node

Contains:
- position
- energy
- capability
- current task status

### Task Node

Contains:
- task type
- execution time
- priority
- status
- constraints

## Edge Types

### UAV-Task Edge

Represents capability matching and execution constraints.

Example:

UAV1 -- Task1

means UAV1 may execute Task1.

### Task-Task Edge

Represents task dependency and execution order.

Example:

Task1 -> Task2

means Task1 must be completed before Task2.

## Core Idea

The graph is not only storing node features. It explicitly preserves relationships that are important for task allocation.
