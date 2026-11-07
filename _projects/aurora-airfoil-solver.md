---
title: Aurora — 2D Airfoil Analysis Solver
description: Development of a Python-based aerodynamic analysis tool combining a vortex panel method with viscous corrections.
order: 4
status: In Progress
tools: Python, NumPy, Matplotlib, Numerical Methods
focus: Computational Aerodynamics and Engineering Software
---

## Overview

Aurora is an independently developed, Python-based
airfoil analysis tool designed to predict the
aerodynamic characteristics of two-dimensional
airfoil geometries.

The project implements a vortex panel method for
inviscid flow analysis and incorporates viscous
corrections to improve aerodynamic performance
predictions.

The objective is to develop a computational tool
that can analyze multiple airfoil geometries,
generate aerodynamic performance data, and compare
results against established reference solutions.

## Engineering Objectives

- Implement a two-dimensional vortex panel method.
- Calculate surface pressure distributions.
- Predict aerodynamic lift and moment coefficients.
- Incorporate viscous corrections into the solver.
- Investigate boundary-layer transition and separation.
- Generate lift, drag, and moment coefficient plots.
- Compare numerical predictions against reference data.

## Engineering Approach

### Airfoil Geometry and Discretization

Airfoil geometries are discretized into a series
of surface panels to approximate the airfoil
boundary and establish the computational domain.

![Airfoil Geometry]({{ '/assets/projects/aurora-airfoil-solver/01_geometry.png' | relative_url }})

*Figure 1. Airfoil geometry used in Aurora.*

### Vortex Panel Method

The solver uses a vortex panel formulation to
calculate the velocity field around an airfoil
under specified freestream conditions.

The resulting surface pressure distribution is
used to evaluate aerodynamic performance.

### Viscous Corrections

Viscous correction methods are incorporated to
estimate aerodynamic behavior not captured by
the inviscid panel method alone.

The analysis considers boundary-layer behavior
and its influence on aerodynamic performance.

### Data Processing and Visualization

Python-based post-processing tools are used to
generate aerodynamic coefficient plots and
compare results across multiple airfoil geometries.

## Results and Validation

### Lift Curve

The lift curve describes the variation in lift
coefficient with angle of attack.

![Lift Curve]({{ '/assets/projects/aurora-airfoil-solver/03_cl_alpha.png' | relative_url }})

*Figure 2. Lift coefficient as a function of angle of attack.*

### Pressure Coefficient Distribution

The pressure coefficient distribution illustrates
the aerodynamic loading across the airfoil surface.

![Pressure Distribution]({{ '/assets/projects/aurora-airfoil-solver/02_cp_distribution.png' | relative_url }})

*Figure 3. Surface pressure coefficient distribution.*

### Solver Validation

Aurora predictions are compared against reference
aerodynamic data to assess the solver's accuracy.

![Solver Validation]({{ '/assets/projects/aurora-airfoil-solver/01_cl_alpha_validation.png' | relative_url }})

*Figure 4. Comparison of Aurora predictions against reference data.*

## Challenges and Lessons Learned

*Numerical implementation challenges, solver
limitations, and validation findings will
be documented here.*

## Technical Documentation

*Source code, technical documentation,
and supporting plots will be added.*
