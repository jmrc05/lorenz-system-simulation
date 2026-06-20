# Lorenz Attractor & Butterfly Effect Simulation

<div align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white" alt="Numpy" />
  <img src="https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge&logo=python&logoColor=white" alt="Matplotlib" />
  <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white" alt="Jupyter Notebooks" />
</div>

---

## Overview

This repository presents a computational and mathematical analysis of the Lorenz chaotic system. The project explores deterministic chaos, the butterfly effect, and the extreme sensitivity to initial conditions inherent in non-linear dynamical systems. 

To guarantee absolute control over numerical stability, local truncation errors, and step size, the integration is performed through a custom-built 4th-order Runge-Kutta (RK4) algorithm, explicitly avoiding reliance on external black-box solvers.

## Mathematical Foundation

The core numerical engine models the Lorenz system, defined by the following set of non-linear ordinary differential equations:

* dx/dt = σ(y - x)
* dy/dt = x(ρ - z) - y
* dz/dt = xy - βz

Analytical inversion of the Jacobian matrix is implemented within the algorithm to optimize the iterative efficiency of the solver and ensure strict convergence.

## Execution and Installation

Clone the repository and install the scientific computing dependencies:

git clone https://github.com/jmrc05/lorenz-system-simulation.git
cd lorenz-system-simulation
pip install numpy matplotlib jupyter

Launch the computational environment to analyze the time series, 3D trajectories, and planar projections:

jupyter notebook practicaEfectoMariposa_MGS_JMRC.ipynb

## Authors

* Juana Maria Rascon Contreras 
* Miriam Garcia Sollo 

Research and algorithmic implementation developed for the Numerical Methods II curriculum.
