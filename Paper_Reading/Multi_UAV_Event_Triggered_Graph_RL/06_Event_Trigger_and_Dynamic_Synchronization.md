# Event Trigger and Dynamic Synchronization

## Event Trigger

The event in this paper refers to important environmental changes that require replanning.

Examples:

- UAV failure
- new task arrival
- task cancellation
- communication changes

## Why Event Trigger?

Continuous replanning causes unnecessary communication and computation costs.

Event-driven planning only updates when meaningful changes occur.

## Dynamic Synchronization

After an event occurs, the system updates:

- UAV states
- Task states
- Graph structure
- Action constraints

Then the framework rebuilds the representation and runs GPPO again.

## Important Difference

Event Trigger answers:

"When should we update?"

Dynamic Synchronization answers:

"How should the world state be updated?"
