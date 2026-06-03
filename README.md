# FinFET vs GAA Nanosheet FET vs NC-FET — Python Simulation & Data

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/cyrilrobinson/finfet-gaa-ncfet-comparison/blob/main/FinFET_GAA_NCFET_Complete.ipynb)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview
Complete Python compact-model simulation comparing **FinFET**, **GAA Nanosheet FET**,
and **Ferroelectric NC-FET** architectures at the 14 nm node with Si, SiGe, and Ge
channel materials, plus 5 advanced composite nano-materials.

**Paper:** "Material Characterization and Performance Comparison of FinFET, GAA
Nanosheet FET, and Ferroelectric NC-FET with Advanced Composite Channel Materials"
*Dr. Cyril Robinson Azariah J., Sir MVIT, Bangalore, India*

## Repository Structure
```
finfet-gaa-ncfet-comparison/
├── FinFET_GAA_NCFET_Complete.ipynb   ← Google Colab notebook (run directly)
├── FinFET_GAA_NCFET_Complete.py      ← Plain Python script
├── figures/                           ← All 12 figures at 300 DPI
│   ├── Fig01_ID_VGS_Transfer.png
│   ├── Fig02_ID_VDS_Output.png
│   ├── Fig03_SubthresholdSwing.png
│   ├── Fig04_DIBL_Bar.png
│   ├── Fig05_Transconductance.png
│   ├── Fig06_ION_IOFF_Ratio.png
│   ├── Fig07_ThresholdVoltage.png
│   ├── Fig08_IOFF_Leakage.png
│   ├── Fig09_PowerDissipation.png
│   ├── Fig10_NCFET_SS_vs_tFE.png
│   ├── Fig11_NanoMaterial_Properties.png
│   └── Fig12_Radar_Performance.png
├── data/                              ← CSV data tables
│   ├── Table1_Performance_Summary.csv
│   ├── Table2_Material_Parameters.csv
│   ├── Table3_Nano_Materials.csv
│   └── Table4_NCFET_GateStack.csv
├── paper/
│   └── main.tex                       ← Springer LaTeX manuscript
├── requirements.txt
└── README.md
```

## Quick Start

### Option 1 — Google Colab (recommended, zero install)
Click the Colab badge above, or open:
```
https://colab.research.google.com/github/cyrilrobinson/finfet-gaa-ncfet-comparison/blob/main/FinFET_GAA_NCFET_Complete.ipynb
```
Then: **Runtime → Run all**

### Option 2 — Local Python
```bash
git clone https://github.com/cyrilrobinson/finfet-gaa-ncfet-comparison
cd finfet-gaa-ncfet-comparison
pip install -r requirements.txt
python FinFET_GAA_NCFET_Complete.py
```

## Key Results Summary

| Device       | SS (mV/dec) | DIBL (mV/V) | ION/IOFF       | IOFF (pA/µm) |
|-------------|-------------|-------------|----------------|--------------|
| Si FinFET   | 68.0        | 62          | 1.80 × 10⁸     | 5.0          |
| SiGe FinFET | 70.0        | 65          | 8.75 × 10⁷     | 12.0         |
| Ge FinFET   | 73.5        | 68          | 2.50 × 10⁷     | 48.0         |
| Si GAA-NS   | **60.0**    | **27**      | **1.69 × 10⁹** | **0.8**      |
| SiGe GAA-NS | 62.0        | 30          | 6.20 × 10⁸     | 2.5          |
| Ge GAA-NS   | 65.0        | 32          | 2.19 × 10⁸     | 8.0          |

## Citation
If you use this code or data in your research, please cite:

```bibtex
@misc{Azariah2025GitHub,
  author       = {Azariah, Cyril Robinson J.},
  title        = {{FinFET--GAA--NCFET Comparison: Python Simulation Code and Data}},
  year         = {2025},
  publisher    = {GitHub},
  howpublished = {\url{https://github.com/cyrilrobinson/finfet-gaa-ncfet-comparison}},
  doi          = {10.5281/zenodo.XXXXXXX}
}
```

Also cite the companion paper (update with DOI after publication):
```bibtex
@article{Azariah2025Paper,
  author  = {Azariah, Cyril Robinson J. and Rajath, R. and Prithvi, N. S.},
  title   = {Material Characterization and Performance Comparison of {FinFET},
             {GAA} Nanosheet {FET}, and Ferroelectric {NC-FET} with Advanced
             Composite Channel Materials},
  journal = {Journal of Computational Electronics},
  year    = {2025},
  doi     = {10.XXXX/XXXXXXX}
}
```

## License
MIT License — see [LICENSE](LICENSE) for details.
