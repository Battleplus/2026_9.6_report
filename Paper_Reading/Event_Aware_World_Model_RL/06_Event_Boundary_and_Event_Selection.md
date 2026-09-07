# 06 Event Boundary and Event Selection

## Problem

If every small change is treated as an event:

- too much noise
- difficult learning
- model focuses on irrelevant changes

If too few events are detected:

- useful information may be lost

## Generic Event Segmentor (GES)

GES is used to control when event prediction should be emphasized.

It checks event density and avoids overusing event information when events become too frequent.

## Main Trade-off

Too many events:
Observation-like learning, redundant information.

Too few events:
Information loss.

The goal is to keep meaningful changes.

## Research Question

How can an agent identify important changes without losing necessary information?

## Test

Why is event selection a balance problem?
