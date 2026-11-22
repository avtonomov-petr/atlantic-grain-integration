# Crisis Echoes or Arbitrage? Selective Co-movement and Integration of the Atlantic Grain Market, 1729–1914

**Author:** Petr Avtonomov (ORCID: [0009-0003-2816-6782](https://orcid.org))  
**Data Source:** Allen–Unger Global Commodity Prices Database (`doi:10.34894/IPVXMW`)  
**Methodology Reference:** First- and Second-Echelon Spectral Auditing (`doi:10.5281/zenodo.24322572`; `doi:10.5281/zenodo.24332448`)

## Overview
This repository contains the reproducible archival pre-audit, panel construction, statistical diagnostics, figures, and LaTeX manuscript for the empirical historical study *"Crisis Echoes or Arbitrage? Selective Co-movement and Integration of the Atlantic Grain Market, 1729–1914"*.

### Key Empirical Findings
1. **Pre-Steam Episodic Synchronization (1729–1855):** Removing secular monetary trends via logarithmic first differences (\(\Delta \ln X_t\)) shows that eighteenth- and early nineteenth-century European grain co-movement was anchored in a Baltic–North Sea–Channel maritime belt and activated episodically during major subsistence and wartime crises (1799–1802, 1809–1810, 1817–1819, and 1847–1848). Excluding seven crisis transition years reduces shared Mode 1 variance from \(23.7\%\) to \(19.2\%\).
2. **Institutional & Geographic Boundaries:** Prior to 1789, interior and municipally regulated markets (Nancy \(0.2\%\), Strasbourg \(0.3\%\), Leipzig \(0.2\%\)) were decoupled from the maritime grain core (England \(6.9\%\), Konigsberg \(6.5\%\), Poland \(6.3\%\), Douai \(5.9\%\)). After 1789, Strasbourg integrated into commercial European grain flows (\(6.96\%\)), whereas Nancy remained regulated and decoupled (\(0.42\%\)).
3. **Post-1850 Transatlantic Flour Bridge:** North American participation rose from \(1.83\%\) (1791–1855, \(N=27\), against a \(22.22\%\) proportional benchmark) to \(13.87\%\) in silver parity (\(12.37\%\) in gold-standard nominal prices) over 1850–1914 (\(N=19\)), led by `Vermont_Flour` (\(9.70\%\), contemporaneous correlation \(r = +0.602\) with `England_Wheat`), while Pacific perishable goods (`Sydney`, \(3.82\%\)) remained decoupled.

## Repository Structure
```text
├── README.md                                 # Study overview and reproduction guide
├── reproduce_atlantic_grain_study.ipynb      # Self-contained Jupyter/Colab notebook
├── data/
│   └── README.md                             # Instructions to obtain raw data via DOI
├── figures/
│   ├── Figure_1.png                          # Pre-steam Atlantic & European dynamics (1752–1855)
│   ├── Figure_2.png                          # Ancien Régime European grain geography (1729–1789)
│   └── Figure_3.png                          # Selective emergence of the transatlantic market (1752–1914)
└── paper/
    ├── main.tex                              # Complete LaTeX manuscript source
    └── Atlantic_Grain_Market_1729_1914.pdf   # Compiled PDF manuscript
```

## Reproducibility Instructions
1. Download the consolidated dataset archive `doi-10.34894-ipvxmw.zip` from DataverseNL (`doi:10.34894/IPVXMW`) and place it in the root directory (or `data/`).
2. Run `reproduce_atlantic_grain_study.ipynb` (or `python reproduce_atlantic_grain_study.py`) top-to-bottom (`Python >= 3.10`, `numpy`, `pandas`, `scipy`, `statsmodels`, `matplotlib`).
3. The pipeline automatically extracts the archive, applies archival continuity and metrological filters, prints summary statistics (`Table 1`), and generates `Figure_1.png`, `Figure_2.png`, and `Figure_3.png`.
