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

## Large Atlas Bundles (N=256)

Due to GitHub repository file-size limits, the full diagnostic atlas bundles
for N=256 simulations are provided via GitHub Releases.

All N=256 atlas bundles associated with the paper are available in:

## Large Atlas Bundles (N=256)

Due to GitHub repository file-size limits, the full diagnostic atlas bundles
for N=256 simulations are provided via GitHub Releases.

All N=256 atlas bundles associated with the paper are available in:

- **GitHub Release: `atlas-256-v1`**  
  https://github.com/The-mirror-walker/Corridor-Diagnostics-and-Predictive-Small-Ball-Entry-in-3D-Incompressible-Navier-Stokes-Data-Atlases/releases/tag/atlas-256-v1

Each archive corresponds to a single initial-condition family and contains
the complete solver diagnostics required to reproduce the reported figures
and tables, including progress logs, invariant summaries, spectral diagnostics,
corridor/onset reports, and configuration metadata.

The corresponding N=128 atlases and all analysis code are available directly
in this repository.
