# Computational Physics & Numerical Simulations 🌌

A comprehensive collection of interactive physics simulations and numerical models implemented in Python using Jupyter Notebooks. This repository focuses on solving differential equations, implementing numerical algorithms, and visualizing complex physical phenomena.

## 🚀 Table of Contents
* [About the Project](#about-the-project)
* [Repository Structure](#repository-structure)
* [Simulations Overview](#simulations-overview)

## 🎯 About the Project
This repository serves as a personal portfolio of computational physics simulations. The core objective is to move beyond analytical approximations by leveraging computational methods (such as finite difference methods and ODE integrators) to model real-world physical systems and visualize their dynamics through matplotlib plots and animations.

## 📂 Repository Structure
To keep the project organized, the simulations are categorized by their corresponding fields of physics:

```text
├── mechanics/
│   └── dynamics_of_material_point.ipynb
├── astrophysics/
│   └── Halley_comet_simulation.ipynb
├── electrostatics_and_fields/
│   └── Poisson_equation_part_1.ipynb
├── waves/
│   └── string_wave_equation.ipynb
├── requirements.txt
└── README.md

```
## 🔬 Simulations Overview

### 1. Dynamics of a Material Point
* 📂 **Path:** `mechanics/dynamics_of_material_point.ipynb`
* 🌌 **The Physics:** This notebook explores classical mechanics by modeling the motion of a particle subjected to various force fields (e.g., constant gravity, linear drag, and harmonic potentials). It simulates how kinematic variables evolve under Newton's second law.
* 🧮 **Numerical Approach:** Implements standard Ordinary Differential Equation (ODE) integration techniques, comparing basic **Euler's method** with more stable solvers like **Runge-Kutta 4th Order (RK4)**.
* 📊 **Key Visualizations:** Generates trajectory plots, velocity-time profiles, and phase space diagrams ($x$ vs $v$) illustrating chaotic or periodic behaviors.

---

### 2. Halley's Comet Orbit Simulation
* 📂 **Path:** `astrophysics/Halley_comet_simulation.ipynb`
* 🌌 **The Physics:** Models the gravitational interaction in a two-body system using Newton's law of universal gravitation. It simulates the highly elliptical orbit (high eccentricity) of Halley's Comet around the Sun, demonstrating Kepler's laws of planetary motion.
* 🧮 **Numerical Approach:** Solves the coupled second-order differential equations of motion in 2D space. It utilizes time-adaptive stepping or energy-conserving integrators (like the **Verlet algorithm** or RK4) to handle the massive speed spikes at the perihelion.
* 📊 **Key Visualizations:** An interactive orbital path plot showing the positions of the Sun and the comet, along with velocity vector changes and kinetic/potential energy conservation graphs.

---

### 3. Poisson's Equation Solver (Part 1)
* 📂 **Path:** `electrostatics_and_fields/Poisson_equation_part_1.ipynb`
* 🌌 **The Physics:** Solves Electrostatic boundary value problems defined by Poisson's partial differential equation ($\nabla^2 \phi = -\frac{\rho}{\varepsilon_0}$). It models the electric potential ($\phi$) distribution in space given a specific distribution of electric charges ($\rho$).
* 🧮 **Numerical Approach:** Discretizes the continuous continuous domain into a 2D grid using the **Finite Difference Method (FDM)**. The resulting linear system is solved iteratively using relaxation techniques such as the **Jacobi method**, **Gauss-Seidel method**, or **Successive Over-Relaxation (SOR)**.
* 📊 **Key Visualizations:** 2D heatmaps/contour plots representing electric potential levels, combined with quiver (vector) plots visualizing the resulting Electric Field ($\vec{E} = -\nabla \phi$).

---

### 4. String Wave Equation Model
* 📂 **Path:** `waves/string_wave_equation.ipynb`
* 🌌 **The Physics:** Simulates the dynamics of a continuous vibrating string fixed at both ends, governed by the 1D hyperbolic Partial Differential Equation (PDE): $\frac{\partial^2 u}{\partial t^2} = v^2 \frac{\partial^2 u}{\partial x^2}$.
* 🧮 **Numerical Approach:** Uses a second-order central difference scheme in both space and time. It respects the **CFL (Courant-Friedrichs-Lewy) stability criterion** to prevent numerical explosion.
* 📊 **Key Visualizations:** Time-evolution surface plots (3D mesh plots showing displacement over space and time) or animated 2D lines representing standing waves, fundamental harmonics, and wave reflections at fixed boundaries.
