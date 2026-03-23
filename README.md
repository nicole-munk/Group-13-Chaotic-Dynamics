# PHAS0052 Physics Group Project 2025-26
# Group 13: Chaotic Dynamics

## Project Files & Authors
* **File:** `Lorenz and Rossler Parameters.ipynb`
  * **Author:** EE
* **File:** `Initial Benchmarking.ipynb`
  * **Author:** EE
* **File:** `Further Benchmarking.ipynb`
  * **Author:** CC
* **File:** `Lorenz bifurcations.ipynb`
  * **Author:** AA
* **File:** `Lorenz_T.ipynb`
  * **Author:** DD
* **File:** `Rossler Hopf bifurcation.ipynb`
  * **Author:** AA
* **File:** `Rossler_TBJ.ipynb`
  * **Author:** DD & AA
* **File:** `calculating_lyapunov_exponent_and_time_for_lorentz_and_rossler.ipynb`
  * **Author:** BB
* **File:** `lyapunov_exponent_solver_comparison.ipynb`
  * **Author:** BB
* **File:** `solvercomparison_bifurcation.ipynb`
  * **Author:** DD

---

## Overview
This repository contains a comprehensive analysis of continuous-time chaotic systems, combining analytical stability techniques with robust numerical simulations. The project investigates the fundamental non-linear dynamics and sensitive dependence on initial conditions inherent to chaotic models. By benchmarking manually implemented numerical solvers against professional algorithms, the project validates the computational methods required to accurately generate phase space trajectories, plot bifurcation diagrams, and calculate Lyapunov exponents.

## Systems Analysed
* **The Rössler System:** Analysed to observe the classic period-doubling route to chaos. The system's topological transitions and equilibrium points were evaluated across varying parameter regimes.
* **The Lorenz System:** Modelled to investigate rapid chaotic divergence, strange attractors, and high-curvature phase space dynamics, alongside an analytical review of its fixed points.

## Key Features & Methodology
* **Analytical Stability Analysis:** * Calculation of equilibrium fixed points for the dynamical systems.
    * Use of Jacobian matrices and eigenvalue evaluation to mathematically determine the stability of these fixed points before simulating.
* **Numerical Methods & Benchmarking:** * Implementation of fundamental numerical integrators: Euler (1st Order), Heun's Predictor-Corrector (2nd Order), and Runge-Kutta 4 (4th Order).
    * Rigorous error analysis and convergence testing to establish theoretical accuracy limits.
    * Performance comparison between the fixed-step manual RK4 method and SciPy’s adaptive `solve_ivp` (`RK45`) solver.
* **Characterising Chaos:**
    * **Bifurcation Diagrams:** Mapping the long-term behaviour of the systems as key parameters are continuously varied, revealing structural transitions into chaos.
    * **Lyapunov Exponents:** Calculation of the Maximal Lyapunov Exponent (MLE) to quantify the exact rate of trajectory divergence and formalise the system's sensitivity to initial conditions.
    * **Phase Space Visualisation:** Generating 3D plots of strange attractors to visually verify the global topology captured by the numerical solvers.

## Technologies Used
* Python 3
* NumPy
* SciPy
* Matplotlib
