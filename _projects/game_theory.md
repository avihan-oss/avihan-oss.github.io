---
layout: page
title: Game Theory & Dynamical Systems
description: Analyzing the stability of Nash Equilibria using Gradient, Replicator, and BNN differential dynamics.
img: /assets/img/game_theory.jpg
importance: 3
category: work
---

## Project Overview
This project bridges the gap between static game theory concepts and dynamic mathematical modeling. [cite_start]Grounded in the foundational texts of **Martin Osborne**, this work extends into the realm of **differential equations** and **control theory** to simulate how strategic interactions evolve over time[cite: 22, 23].

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/game_theory.jpg" title="Phase Portrait of Replicator Dynamics" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Simulating evolutionary stability in the Hawk-Dove game using Replicator Dynamics.
</div>

### Key Mathematical Models
We investigated four distinct dynamical systems to test the stability of equilibrium points:

#### 1. Cournot Oligopoly & Gradient Dynamics
* [cite_start]**Static Model**: Derived the N-Firm Cournot equilibrium where $P^* \to \text{Average Cost}$ as $N \to \infty$[cite: 123].
* **Dynamic Stability**: Modeled the adjustment process using **Gradient Adjustment Dynamics**:
    $$\dot{q}_i(t) = k_i \frac{\partial \pi_i}{\partial q_i}$$
* [cite_start]**Result**: Proved via Jacobian analysis that the Cournot Nash Equilibrium is a **globally asymptotically stable sink** ($\text{Trace}(A) < 0, \text{Det}(A) > 0$)[cite: 169, 173].

#### 2. Evolutionary Games & Replicator Dynamics
* [cite_start]Applied to the **Hawk-Dove Game** and **Matching Pennies**[cite: 246, 202].
* Utilized the **Replicator Equation** to model population shifts based on payoff differences:
    $$\dot{x}_i = x_i [u(e_i, x) - \bar{u}(x)]$$
* [cite_start]**Result**: Demonstrated that the Mixed Strategy Nash Equilibrium is an **Evolutionarily Stable Strategy (ESS)** and a stable attractor[cite: 262].

#### 3. Differential Games (Stackelberg)
* Modeled sequential interactions continuously over time using **Control Theory**.
* [cite_start]Solved for **Feedback Stackelberg Solutions** using **Hamilton-Jacobi-Bellman (HJB)** equations to ensure time-consistency and subgame perfection[cite: 336, 337].

#### 4. Coalitional Games & The Core
* Investigated cooperative games where players form binding agreements.
* [cite_start]**BNN Dynamics**: Modeled the negotiation process using **Brown-von Neumann-Nash dynamics**, proving that trajectories converge to **The Core** from any efficient initial allocation[cite: 385, 395].

### Technical Implementation
* [cite_start]**Proofs**: Validated existence of equilibria using **Kakutani’s Fixed Point Theorem**[cite: 61].
* [cite_start]**Simulation**: Built computational engines in **Python** and **MATLAB** to generate phase portraits and vector fields for the dynamical systems[cite: 30].
