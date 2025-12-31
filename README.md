# Corridor-Diagnostics-and-Predictive-Small-Ball-Entry-in-3D-Incompressible-Navier-Stokes-Data-Atlases

This repository accompanies the paper:

**Corridor Diagnostics and Predictive Small-Ball Entry in 3D Incompressible Navier–Stokes: An Empirical Atlas Study**

[arXiv link]

It provides the diagnostic atlas bundles, solver outputs, and supporting data
used in the analysis.

---

## Repository Structure

- `DYADIC_TOWER_complete_N128/` — Full diagnostic atlas for the dyadic tower
  initial condition at resolution N=128.
- `DYADIC_TOWER_WF_spread_N128/` — Window length and fractional threshold
  sweep demonstrating detector robustness for the same trajectory.

## Procedural Initial Conditions

The ABC, TG, TG2X, and RAND_SOL initial conditions are generated internally by
analytic or stochastic constructions embedded directly in the solver.

Each realization is uniquely determined by the recorded configuration:
(IC type, IC parameters, grid resolution N, energy normalization E0, and RNG seed).
No external initial-condition files are required for reproducibility.

For transparency and inspection only, representative initial velocity fields
at t = 0 are provided for selected runs. These snapshots are not required to
reproduce the results reported in the paper.
