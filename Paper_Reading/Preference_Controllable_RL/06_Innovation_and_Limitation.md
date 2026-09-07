# Innovation and Limitation

## Main Innovations

### 1. Preference Controllable Policy

Instead of training one policy for one preference, PCRL learns a single policy conditioned on preference input.

### 2. Integration with Advanced MOO

The framework can incorporate existing multi-objective optimization algorithms.

### 3. PreCo Algorithm

PreCo jointly considers:

- Pareto optimization
- Preference alignment
- Gradient conflict handling

## Limitations

### 1. Preference Space Assumption

The method assumes preferences can be represented as objective weights.

### 2. Computational Cost

Gradient manipulation introduces additional optimization overhead.

### 3. Objective Definition

Performance depends on whether objectives are properly designed.

## Research Value

The paper provides an important bridge between MORL and preference alignment methods.
