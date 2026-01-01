# Corridor Diagnostics and Predictive Small-Ball Entry in 3D Incompressible Navier–Stokes — Data Atlases

This repository accompanies the paper:

**Corridor Diagnostics and Predictive Small-Ball Entry in 3D Incompressible Navier–Stokes: An Empirical Atlas Study**

[arXiv link]

It provides diagnostic atlas bundles, solver outputs, and supporting data
used in the analysis.

---

## Repository Contents (N = 128)

This repository contains the complete diagnostic atlases for simulations
performed at resolution N = 128.

Each atlas is provided as a compressed archive and corresponds to a single
initial-condition family and integration length. Filenames follow the
convention:

```
<IC>.<steps>.N128.ATLAS.zip
<IC>.W.F.N128.window.spread.zip
<IC>.N128.IC_snap_shots.zip
```

where:
- `<IC>` denotes the initial-condition family (ABC, TG, TG2X, Dyadic Tower,
  Max Helix, Traveling Helical Wave, etc.),
- `<steps>` is the total integration length,
- `ATLAS` indicates a full diagnostic bundle,
- `W.F.window.spread` denotes window-length / fractional-threshold robustness sweeps,
- `IC_snap_shots` contains representative velocity and pressure field snapshots
  at t = 0.

All analysis scripts and documentation required to interpret these atlases
are included directly in this repository.

---

## Procedural Initial Conditions

The ABC, TG, TG2X, and RAND_SOL initial conditions are generated internally by
analytic or stochastic constructions embedded directly in the solver.

Each realization is uniquely determined by the recorded configuration:
(IC type, IC parameters, grid resolution N, energy normalization E0,
and RNG seed where applicable). No external initial-condition files are
required for reproducibility.

For transparency and inspection only, representative initial velocity and
pressure fields at t = 0 are provided for selected runs via the
`IC_snap_shots` archives. These files are **not required** to reproduce the
results reported in the paper.

---

## Large Atlas Bundles (N = 256)

Due to GitHub repository file-size limits, the full diagnostic atlas bundles
for simulations at resolution N = 256 are provided via GitHub Releases.

All N = 256 atlas bundles associated with the paper are available in:

- **GitHub Release: `atlas-256-v1`**  
  https://github.com/The-mirror-walker/Corridor-Diagnostics-and-Predictive-Small-Ball-Entry-in-3D-Incompressible-Navier-Stokes-Data-Atlases/releases/tag/atlas-256-v1

Each archive corresponds to a single initial-condition family and contains
the complete solver diagnostics required to reproduce the reported figures
and tables, including progress logs, invariant summaries, spectral diagnostics,
corridor/onset reports, and configuration metadata.

The corresponding N = 128 atlases and all analysis code are available
directly in this repository.
