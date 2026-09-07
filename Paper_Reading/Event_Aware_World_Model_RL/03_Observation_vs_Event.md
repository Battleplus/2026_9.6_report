# 03 Observation vs Event

## Observation
Observation is the raw information received from the environment.

Example:
- Image pixels
- Robot joint values
- Object categories

## Event
Event represents meaningful changes in observations.

Examples:
- Object movement
- Velocity change
- Category change

## Important Difference

Paper 1:
Event = trigger for decision update or replanning.

Paper 2:
Event = representation of meaningful environmental changes used for world model learning.

## Important Understanding
EAWM does not remove observations.

It keeps observation prediction and adds event prediction as an additional learning objective.

## Why Events?
Raw observations contain redundant information. Events provide compact information about dynamic changes.
