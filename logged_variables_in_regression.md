# Logged variables in regression

**Author:** Alun Hughes
**Version:** 1.0
**Date:** November 2025

## Introduction

In the regression relationship $y = b \ln(x) + c$, the coefficient $b$ can be interpreted as a rate of change, e.g. the *unit change in y for a percentage change in x*. This is called the **semi-elasticity** in economics.

## Derivation

The interpretation of $b$ as a rate of change can be derived using calculus:

1.  **Differentiate the function**: To find the instantaneous rate of change of *y* with respect to *x*, take the derivative of the equation with respect to ${x}$:

    $\frac{dy}{dx} = \frac{d}{dx}(b \ln(x) + c)$

    $\frac{dy}{dx} = b \cdot \frac{1}{x}$
  
    $\frac{dy}{dx} = \frac{b}{x}$

3.  **Rearrange the derivative**: The term $\frac{dy}{dx}$ represents the change in $y$ for a one-unit change in $x$. Rearranging the equation gives:

    $b = x \cdot \frac{dy}{dx}$

    $b = \frac{dy}{\frac{dx}{x}}$

5.  **Interpretation**:
    *   $dy$ is the change in ${y}$ (in units of ${y}$).
    *   $\frac{dx}{x}$ is the *proportional* or *percentage* change in $x$ (since $\frac{dx}{x} \times 100$ is the percentage change).

Therefore, $b$ is the ratio of the unit change in $y$ to the proportional change in $x$.

### Practical Interpretation

In practical terms, for the model $y = b \ln(x) + c$,

*   A **one percent increase in $x$** is associated with a change of approximately **$b/100$ units in $y$**, on average, holding all other variables constant.
*   Alternatively, you can state that a **one unit increase in $\ln(x)$** is associated with a **$b$ unit change in $y$**.

This makes $b$ a useful measure of the association between $y$ and *relative* changes in $x$, which is often pertinent in economic or biomedical contexts (e.g., the relationship between a percentage change in income and the absolute level of consumption or the relationship between a percentage change in NT-proBNP and walking distance).
