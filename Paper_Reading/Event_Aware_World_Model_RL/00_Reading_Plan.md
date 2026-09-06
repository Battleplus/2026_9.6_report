# Event-Aware World Model for Reinforcement Learning Reading Plan

## Purpose

This folder is prepared for continuing the second paper study with the same learning framework used for the Multi-UAV Event-Triggered Graph RL paper.

The goal is not only to summarize the paper, but to understand:

- Why the method is proposed.
- What problem the previous methods cannot solve.
- How each module contributes.
- How training works.
- What are the advantages and limitations.

## Recommended Learning Order

### 01. Paper Overview

Explain:

- Research background
- Main problem
- Core contribution
- Overall framework

### 02. World Model Background

Explain:

- What is a world model?
- Difference between model-free RL and model-based RL.
- Why prediction of environment dynamics is useful.

### 03. Observation vs Event

Focus on:

- What is observation?
- What is event?
- Why not process every observation?
- Why important changes should be extracted?

### 04. Event Representation

Explain:

- How events are detected.
- How meaningful changes are represented.
- How event information differs from raw observation.

### 05. Event-Aware World Model Architecture

Analyze:

- Each module input/output.
- Information flow.
- Training objective.

### 06. Event Boundary and Event Selection

Discuss:

- How event boundaries are defined.
- How useful changes are selected.
- Risk of filtering useful information.

### 07. Reinforcement Learning Integration

Explain:

- How the world model interacts with RL policy.
- What parameters are updated during training.
- Training stage versus deployment stage.

### 08. Experiments

Analyze:

- Baselines.
- Metrics.
- Ablation experiments.
- Why results support the method.

### 09. Strengths and Limitations

Prepare:

- Research contribution.
- Possible weaknesses.
- Future improvement directions.

### 10. Comparison With Paper 1

Compare:

Paper 1:
Event triggers replanning in multi-UAV task allocation.

Paper 2:
Event helps the world model understand meaningful environmental changes.

## Required Outputs

For every section:

1. Markdown notes.
2. One independent PPT-style figure.
3. Question-answer test to check understanding.
4. Final conclusion summary.
