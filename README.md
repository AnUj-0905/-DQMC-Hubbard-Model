# DQMC

![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/drazerd/dqmc)
![GitHub license](https://img.shields.io/github/license/drazerd/dqmc)

Efficient and stable Determinant Quantum Monte Carlo (DQMC) simulations of the Hubbard model in Python.

| :warning: WARNING: This project is still under active development and may change significantly in future versions! |
|--------------------------------------------------------------------------------------------------------------------|

| ℹ️ This version uses a pure Python + Numba backend. Fortran acceleration has been removed for simpler installation and maintenance. |

---

## Features

- Pure Python implementation
- Numba JIT acceleration
- Stable ASvQRD matrix stabilization
- Determinant Quantum Monte Carlo for Hubbard model
- Multiprocessing support
- Equal-time observable measurements

---

## Installation

Install directly from GitHub:

```commandline
pip install git+https://github.com/drazerd/dqmc.git
```

---

## Hubbard Model Project — IISER Bhopal

This repository contains the DQMC codebase used for a computational study of the
two-dimensional Hubbard model at half filling, along with the associated project
report and numerical results.

### Project scope

- Square lattice with periodic boundary conditions.
- Main simulations on a \(4\times4\) lattice.
- Hopping amplitude \(t=1\).
- Interaction strengths \(U/t=0,\ldots,8\).
- Inverse temperature \(\beta=4\), with imaginary-time step \(\Delta\tau=0.1\).
- Observables: double occupancy, local magnetic moment, and interaction energy.
- A \(2\times2\) exact-diagonalization comparison was used to validate the DQMC results.

### Report

The `report/` directory contains the project report, LaTeX source, bibliography,
plot files, and supporting style files.

The report is titled *Determinant Quantum Monte Carlo Simulation of the 2D Hubbard
Model* and credits Dhruv Dua, Dumbre Anuj, and Ishit Ranjan (IISER Bhopal).

### Code provenance and attribution

This project builds on the DQMC implementation developed by Dylan Jones:
https://github.com/dylanljones/dqmc

The upstream implementation is distributed under the MIT License. Its original
license and copyright notice are retained in this repository. Project-specific
changes, simulation work, analysis, and report content should be distinguished
from the upstream implementation.

See `LICENSE` for the applicable license terms.
