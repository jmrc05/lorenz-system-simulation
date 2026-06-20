# Lorenz Attractor & Butterfly Effect Simulation 🦋

<div align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white" alt="Numpy" />
  <img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter Notebooks" />
</div>

---

## Overview

This repository presents a computational and mathematical analysis of the Lorenz chaotic system. The project explores the butterfly effect and the extreme sensitivity to initial conditions inherent in non-linear dynamical systems. 

To guarantee absolute control over numerical stability, local truncation errors, and step size, the integration is performed through a custom-built 4th-order Runge-Kutta (RK4) algorithm instead of relying on external black-box solvers.

## Mathematical Foundation

The Lorenz system is defined by the following set of non-linear ordinary differential equations:

$$ \frac{dx}{dt} = \sigma(y - x) $$
$$ \frac{dy}{dt} = x(\rho - z) - y $$
$$ \frac{dz}{dt} = xy - \beta z $$

The numerical core implements analytical inversion of the Jacobian matrix to optimize the iterative efficiency of the solver and ensure convergence.

## Visual Results

Executing the core notebook generates the following analytical representations:
* 3D rendering of the global geometry of the strange attractor.
* Planar projections mapped over the xy and xz axes.
* Fractal maps illustrating the domains of attraction.

<div align="center">
  <img src="docs/lorenz_attractor.png" alt="3D Lorenz Attractor rendering" width="70%" />
</div>

## Installation and Usage

Clone the repository and install the scientific dependencies:

```bash
git clone [https://github.com/jmrc05/lorenz-attractor-rk4.git](https://github.com/jmrc05/lorenz-attractor-rk4.git)
cd lorenz-attractor-rk4
pip install numpy matplotlib jupyter
