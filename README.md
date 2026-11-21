# First-Principles Quantum Hydrodynamics, Chiral Spin-2 Gravitons, Primordial Nucleosynthesis, and Dual Empirical Calibration of the Cosmic Superfluid Crystallization Threshold ($\chi_{\text{crit}}$)
[![DOI](https://zenodo.org/badge/1466946412.svg)](https://doi.org/10.5281/zenodo.24430134)
**Author:** Ehab Mohamed Abdel Gwad Manse  
**Affiliation:** Independent Theoretical Physics Researcher, Cairo, Egypt  
**ORCID:** [0009-0009-4846-6188](https://orcid.org)  
**Contact:** ehabmanse2@gmail.com  

---

## Overview

This repository contains the reproducible Python/Jupyter computational simulations and numerical ODE/PDE solvers accompanying the second paper in the **Unified Quantum Superfluid Cosmology** series. The codebase numerically validates:

1. **CMB Angular Power Spectrum ($C_\ell$) & 12-Reaction Primordial Nucleosynthesis (BBN):** Direct wavenumber ($k$) integration of the Bogoliubov–Boltzmann acoustic transfer spectrum inside a topologically closed superfluid cavity alongside a stiff Log-Temperature LSODA solver for the 12 primary nuclear reaction rates ($^4\mathrm{He}$, $\mathrm{D}$, $^3\mathrm{He}$, $^7\mathrm{Li}$).
2. **3D Quantum Hydrodynamic Crystallization Across *The Barzakh*:** A 3D Split-Step Fourier Method (SSFM) solver for the coupled time-dependent Gross–Pitaevskii–Poisson system demonstrating spontaneous symmetry breaking above $\chi_{\text{crit}} = 4.2 \times 10^4$ stabilized by quantum Bohm pressure within the healing length $\xi = 4.16\,\mathrm{kpc}$.
3. **Dynamical Black Hole Phase-Shear Recycling Engine (Axiom 8):** Simulation of gravitational core compression across the critical Higgs phase-shear threshold ($\chi_{\text{shear}} = 2.5 \times 10^5$), demonstrating barrier collapse and non-singular quantum Bohm bounce back into ground-state $\rho_{\text{DM}}$.
4. **Peripheral Galactic Gas Turbulence & Rotation Curve Flattening:** Radial hydrodynamic integration reproducing the universal $\sigma_{\text{edge}} \approx 7.14\,\mathrm{km/s}$ outer disk velocity dispersion floor and asymptotic rotation velocity flattening ($V_{\text{rot}} = 152.2\,\mathrm{km/s}$ vs. $122.8\,\mathrm{km/s}$ Keplerian).
5. **Environmental BAO Scale Shift & Hemispherical Dipole Anisotropy:** Full-sky angular modulation and void-vs.-cluster sound-horizon splitting ($\Delta r_d / r_d = \pm 0.75\%$ environmental; $\pm 7.95\%$ directional) aligned with the CMB dipole axis $(l, b) \approx (221^\circ, -20^\circ)$.

---

## Repository Structure

| Notebook / Script | Paper Section | Output Figure | Key Computed Benchmark |
| :--- | :--- | :--- | :--- |
| `Sim_01_CMB_and_12ODE_BBN.ipynb` | Section 3 (Eqs. 7–8) | `cmb_simulation.png` | $D_2 = 95.7\,\mu\mathrm{K}^2$ (vs. $220.8\,\Lambda\mathrm{CDM}$); $Y_p = 0.241$, $\mathrm{D/H} = 1.85\times 10^{-5}$, $^7\mathrm{Li/H} = 3.46\times 10^{-10}$ |
| `Sim_02_3D_GPE_Crystallization.ipynb` | Section 7.1 (Table 4) | `sim1_3d_crystallization.png` | $\chi_{\text{peak}} = 4.97 \times 10^4 > \chi_{\text{crit}}$; Core mean $4.68 \times 10^4$ ($r \le 4.16\,\mathrm{kpc}$); Crystallized volume $1.27\%$ |
| `Sim_03_Black_Hole_Recycling.ipynb` | Section 7.2 (Table 5) | `sim2_bh_recycling.png` | Peak $\chi = 2.76 \times 10^5$ (Step 55) $\to$ Non-singular relaxation $\chi = 1.58 \times 10^4$ (Step 200) |
| `Sim_04_Galactic_Edge_and_Rotation.ipynb` | Section 7.3 (Table 6) | `sim3_galaxy_edge.png` | $\sigma_{\text{UDF}}(25\,\mathrm{kpc}) = 7.14\,\mathrm{km/s}$ (vs. $0.28\,\mathrm{km/s}$ std); $V_{\text{rot}} = 152.2\,\mathrm{km/s}$ |
| `Sim_05_BAO_Directional_Anisotropy.ipynb` | Section 7.4 (Table 7) | `sim4_bao_anisotropy.png` | $r_d = 145.99\,\mathrm{Mpc}$ (Cluster) vs. $148.19\,\mathrm{Mpc}$ (Void); $135.40\text{--}158.78\,\mathrm{Mpc}$ dipole |

---

## Installation & Execution

All notebooks are self-contained and run directly on **Google Colab** or any local Python 3.10+ environment:

```bash
pip install numpy scipy matplotlib
```

Run each `.ipynb` notebook sequentially from top to bottom to reproduce all high-resolution figures (`300 DPI`) and printed numerical verification tables reported in the manuscript.

---

## Citation

If you use these derivations, empirical calibrations, or simulation codes in your research, please cite:

```bibtex
@article{Manse2026_SuperfluidThreshold,
  author  = {Manse, Ehab Mohamed Abdel Gwad},
  title   = {First-Principles Quantum Hydrodynamics, Chiral Spin-2 Gravitons, Primordial Nucleosynthesis, and Dual Empirical Calibration of the Cosmic Superfluid Crystallization Threshold (\(\chi_{\text{crit}}\))},
  year    = {2026},
  month   = {November},
  note    = {ORCID: 0009-0009-4846-6188}
}
```

