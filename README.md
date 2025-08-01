# Bisection Method Implementation

A simple implementation of the bisection method for finding roots of continous functions.

## Overview
The bisection method is a simple root-finding algorithm that works by repeatedly dividing an interval in half and selecting the subinterval that contains the root.

### How it works

1. Start with an interval `[a, b]` where `f(a)` and `f(b)` have opposite signs
2. **Iteration**:
    - Calculate the midpoint `c = (a+b) / 2`
    - Evaluate `f(c)`
    - If `|f(c)| < tolerance`, `c` is a close approximation for a root.
    - Otherwise, replace `a` or `b` with `c` based on the sign of `f(c)`

### Math

For a continous function `f(x)` and an interval `[a, b]` where `f(a) * f(b) < 0`, the [Intermediate Value Theorem](https://en.wikipedia.org/wiki/Intermediate_value_theorem) guarantees that there exists at least one root in the interval. The bisection method uses this property to approach the root.

## Licence
This project is open source and available under the GNU GPL Licence.