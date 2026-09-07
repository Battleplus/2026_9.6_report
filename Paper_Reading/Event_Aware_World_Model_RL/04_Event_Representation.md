# 04 Event Representation

## Event Generation

The paper automatically generates events without manual labels.

Different observation types use different event definitions:

- Visual input: changes in brightness or visual patterns.
- Ordinal data: changes exceeding thresholds.
- Nominal data: category changes.

## Event Predictor

The world model predicts:

1. Future observations.
2. Future events.

Event prediction helps the model focus on meaningful spatio-temporal transitions.

## Representation Learning

Observation provides information.
The representation model converts information into latent states.
Event prediction improves the learned representation.

## Key Point
Event is not the latent representation itself. It is an auxiliary learning signal.
