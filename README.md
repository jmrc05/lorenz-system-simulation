# Lorenz Attractor & Butterfly Effect Simulation

Numerical simulation of the Lorenz chaotic system exploring the butterfly effect through the classical 4th-order Runge-Kutta (RK4) method.

## Overview

This repository contains a rigorous mathematical and computational analysis of the Lorenz system. By implementing the RK4 method from scratch, the simulation visualizes deterministic chaos and the extreme sensitivity to initial conditions inherent in non-linear dynamical systems.

## Mathematical Foundation

The Lorenz system is modeled by a set of three coupled, non-linear ordinary differential equations:

* `dx/dt = σ(y - x)`
* `dy/dt = x(ρ - z) - y`
* `dz/dt = xy - βz`

Instead of relying on black-box external solvers, the numerical integration is handled via a custom-built 4th-order Runge-Kutta algorithm. This ensures full control over the step size, local truncation error, and overall numerical stability.

## Tech Stack

* **Language:** Python
* **Environment:** Jupyter Notebook
* **Core Libraries:** 
  * `numpy` for high-performance vectorized calculations and matrix operations.
  * `matplotlib` for 3D trajectory rendering and planar projections.

## Visual Results

<!-- Replace the URL below with the actual link to your generated image -->
![Lorenz System 3D Projection](docs/lorenz_attractor_visualization.png)

## Usage and Execution

To run the simulation locally, ensure you have the required dependencies installed:

```bash
pip install numpy matplotlib jupyter
