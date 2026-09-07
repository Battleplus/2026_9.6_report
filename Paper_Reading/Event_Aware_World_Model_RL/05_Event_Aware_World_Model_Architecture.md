# 05 Event-Aware World Model Architecture

## Overall Idea

EAWM does not remove the traditional world model. It adds event prediction as an additional learning objective.

Overall flow:

Observation
↓
Representation Model
↓
Latent State
↓
World Model
↓
Future Prediction

Additional branch:

Latent State
↓
Event Predictor
↓
Future Event Prediction

## Main Modules

### Representation Model

Input: current observation and history.

Output: latent representation of the environment.

It converts raw input into information useful for prediction.

### Sequence Model

It remembers previous states and actions.

Reason:
A single observation cannot describe motion and dynamics.

### Dynamics Predictor

Predicts how latent state changes in the future.

### Observation Predictor

Predicts future observations.

### Event Predictor

Predicts meaningful environmental changes.

The event prediction task helps the model focus on dynamic changes instead of irrelevant visual details.

## Key Understanding

Event is not the replacement of observation.
Event is an additional signal that improves representation learning.

## Test

1. Does EAWM discard raw observation prediction?
2. What is the role of Event Predictor?
