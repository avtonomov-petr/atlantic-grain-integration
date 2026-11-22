# Data Source Instructions

This study uses the consolidated **Allen–Unger Global Commodity Prices Database** (Version 1.0):
* **Citation:** Allen, R. C., & Unger, R. W. (2026). *The Allen Unger Commodities Dataset*. DataverseNL. `doi:10.34894/IPVXMW`
* **Direct Link:** https://doi.org

## How to Reproduce
1. Download the archive `doi-10.34894-ipvxmw.zip` from DataverseNL using the DOI above.
2. Place `doi-10.34894-ipvxmw.zip` into the root folder of this repository (or into `data/`).
3. Run `reproduce_atlantic_grain_study.ipynb` (or `python reproduce_atlantic_grain_study.py`). The script will automatically extract the archive, execute the archival pre-audit filters, and generate all summary tables and figures.

