# 01 Paper Overview

## Paper
From Observations to Events: Event-Aware World Model for Reinforcement Learning

## Core Problem
Existing model-based reinforcement learning methods learn world models mainly by predicting raw observations. However, raw observations contain redundant information such as textures, colors, and background changes.

The paper argues that agents should focus on meaningful environmental changes rather than every pixel.

## Main Idea
EAWM introduces event-aware representation learning:

Observation -> Event -> World Model Representation -> Policy Learning

The goal is not to replace observations with events, but to use event prediction as an additional learning objective.

## Main Contributions

1. Event-aware world model framework.
2. Automated event generation without manual labels.
3. Generic Event Segmentor (GES) for event boundary detection.
4. Improvement on Atari, Craftax, DeepMind Control and DMC-GB2 benchmarks.

## Key Understanding
World Model predicts how the environment changes.
Event prediction helps the model understand which changes matter.

## Questions
1. Why is raw observation prediction insufficient?
2. What is the difference between event in this paper and event-triggered RL?
