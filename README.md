# Optimizing Heat Transfer in Heat Sink Fin Arrays Using CFD 

## Overview
This project investigates the optimization of passive heat sink fin arrays using **Computational Fluid Dynamics (CFD)** to improve natural convection heat transfer performance.

The study analyzed multiple fin configurations to determine the optimal fin spacing that maximizes heat dissipation while minimizing material usage and airflow restriction.

The project was completed as part of the **MCEN 4231/5231 Computational Fluid Dynamics** course at the University of Colorado Boulder. :contentReference[oaicite:0]{index=0}

---

# Project Objective
- Analyze natural convection heat transfer in fin arrays
- Optimize fin spacing for maximum thermal performance
- Study boundary layer interaction between fins
- Compare heat transfer rates across multiple configurations
- Validate CFD-based thermal analysis methods

---

# Project Team
- Surya Sharon Raj Goda
- Saravana Kumar Kodakinti Prakash
- Anoop Subramanya
- K. Vaikunth Keshav

---

# Simulation Configurations

Three different fin configurations were studied while maintaining identical base dimensions. :contentReference[oaicite:1]{index=1}

| Configuration | Number of Fins | Fin Spacing | Heat Transfer Rate |
|---|---|---|---|
| A | 6 Fins | 17.8 mm | 2.85 W |
| B | 10 Fins | 9.3 mm | 4.62 W |
| C | 13 Fins | 6.5 mm | 3.92 W |

---

# Key Results 📊

## Optimal Configuration
The **10-fin configuration** achieved the best thermal performance:
- ✅ 62% higher heat transfer than the 6-fin configuration
- ✅ 18% higher heat transfer than the 13-fin configuration
- ✅ Optimal balance between airflow and surface area

:contentReference[oaicite:2]{index=2}

---

# CFD Methodology

## Governing Physics
The simulation solved:
- Conservation of Mass
- Momentum Equations
- Energy Equations
- Boussinesq Approximation for buoyancy-driven flow

The study used a:
- Monolithic coupling approach
- Crank–Nicolson temporal discretization
- SUPG & PSPG stabilization methods

:contentReference[oaicite:3]{index=3}

---

# Computational Setup

| Parameter | Value |
|---|---|
| Domain Size | 14 cm × 4 cm |
| Fin Height | 2.4 cm |
| Fin Thickness | 5 mm |
| Mesh Type | Unstructured Triangular |
| Mesh Elements | 45,000 – 75,000 |
| Simulation Time | 5 seconds |
| Time Step | 0.0275 s |
| Prandtl Number | 0.7215 |
| Rayleigh Number | 5.69 × 10⁸ |

:contentReference[oaicite:4]{index=4}

---

# Meshing & Numerical Methods

## Mesh Strategy
- Fine mesh refinement near fin surfaces
- Boundary layer resolution using:
  - 0.3 mm mesh size near fins
  - 2.5 mm mesh size in outer regions

## Solvers Used
- DOLFINx
- Newton Solver
- GMRES Linear Solver
- LU Preconditioner
- MPI Parallel Processing

:contentReference[oaicite:5]{index=5}

---

# Boundary Conditions

| Surface | Condition |
|---|---|
| Bottom Surface & Fins | No-slip + Constant Temperature |
| Side & Top Boundaries | Open Boundary |
| Initial Fluid State | Stationary |
| Ambient Temperature | 303 K |
| Fin Temperature | 353 K |

:contentReference[oaicite:6]{index=6}

---

# Engineering Insights

## Boundary Layer Interaction
The study demonstrated that:
- Large spacing reduces surface area utilization
- Very small spacing restricts airflow due to merged thermal boundary layers
- Optimal performance occurs when thermal boundary layers begin interacting without excessive flow restriction

Optimal heat transfer occurred at:
- Rayleigh Number (RaS) ≈ 1 × 10³ to 3 × 10³

:contentReference[oaicite:7]{index=7}

---

# Tools & Software Used

## CFD & Simulation
- DOLFINx
- FEniCS
- MPI Parallel Computing

## Meshing & Preprocessing
- Gmsh

## Post Processing
- CFD Visualization
- Velocity & Temperature Field Analysis

## Engineering Concepts
- Natural Convection
- Heat Transfer
- Thermal Boundary Layers
- Numerical Methods
- Finite Element Analysis

---

# Key Outcomes
- Successfully modeled buoyancy-driven natural convection
- Identified optimal fin spacing for passive cooling
- Validated monolithic CFD coupling methods
- Improved understanding of thermal boundary layer interaction
- Demonstrated practical heat sink optimization methods for electronics cooling

---

# Repository Contents
This repository includes:
- Final Project Report
- CFD Results
- Simulation Images
- Mesh Visualizations
- Temperature & Velocity Fields
- Numerical Methodology
- Engineering Analysis

---

# Applications
- Electronics Cooling
- Thermal Management Systems
- Heat Sink Optimization
- Passive Cooling Design
- Aerospace Thermal Systems
- Automotive Electronics Cooling

---

# Author
**Anoop Subramanya**  
Mechanical Engineer | CFD | Thermal Systems | Mechanical Design

- LinkedIn: www.linkedin.com/in/anoopsubramanya
- Portfolio: https://anoopsubramanya.framer.website/
---
*"Using CFD to optimize thermal performance through engineering-driven design."*
