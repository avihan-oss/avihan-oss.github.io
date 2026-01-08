---
layout: page
title: Prey-Predator Dynamics
description: Modeling ecological stability using Lotka-Volterra differential equations.
img: /assets/img/prey_predator.jpg # You will need to upload an image later
importance: 4
category: work
---

## Project Overview
This project explores the mathematical modeling of interacting species using **Ordinary Differential Equations (ODEs)**. The goal was to analyze the stability of ecological systems where prey and predator populations oscillate over time.

### Mathematical Model
We utilized the classic **Lotka-Volterra equations** to describe the dynamics:

$$
\begin{aligned}
\frac{dx}{dt} &= \alpha x - \beta xy \\
\frac{dy}{dt} &= \delta xy - \gamma y
\end{aligned}
$$

Where:
* $x$: Prey population
* $y$: Predator population
* $\alpha, \beta, \delta, \gamma$: Interaction coefficients representing growth, predation, and death rates.

### Key Analysis
* **Equilibrium Points**: Calculated the fixed points of the system to determine conditions for coexistence versus extinction.
* **Stability Analysis**: Computed the **Jacobian Matrix** and eigenvalues to classify equilibrium points (e.g., centers, spirals, or saddles).
* **Phase Portraits**: Generated phase plane plots to visualize the cyclic nature of the populations.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/prey_predator.jpg" title="Phase Portrait" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Phase portrait showing the cyclic relationship between predator and prey populations.
</div>

### Tools Used
* **MATLAB / Python**: For numerical simulation (Runge-Kutta methods).
* **Dynamical Systems Theory**: For analytical stability proofs.
