## 📘 Topography Dominates the Hemispheric Asymmetry of Stratospheric Sudden Warmings

**Author**: Siming Liu  
**Affiliations**: The University of Chicago  
**Contact**: smliu01@uchicago.edu

### 🔍 Overview

This repository contains the code and analysis for the study:

> **Topography dominates the hemispheric asymmetry of Stratospheric Sudden Warmings**  
> Liu, S., Shaw, T. A., & Garfinkel, C. I. (2025). accepted by Geophysical Research Letters.

The study investigates why **Stratospheric Sudden Warmings (SSWs)** occur almost exclusively in the Northern Hemisphere (NH). Using climate model simulations, the paper shows that **topography is the dominant factor** in creating this hemispheric asymmetry through its control of eddy heat flux.

---

### 📄 Paper

- **Main Manuscript**: [`manuscript.pdf`](./result/manuscript.pdf)  
- **Supporting Information**: [`supplementary.pdf`](./result/supplementary.pdf)

---

### 📂 Notebooks

The analysis is broken into several Jupyter notebooks:

| Notebook | Description |
|----------|-------------|
| `ssw_onset_dm.ipynb` | Detects the onset of SSW events following the Charlton & Polvani (2007) method. |
| `tropos_ssw_v_t_vint.ipynb` | Calculates and visualizes vertically integrated meridional eddy heat flux (`v*T*`) in both hemispheres. |
| `v.t.daily.ipynb` | Computes and analyzes daily zonal deviations of meridional wind (`v`) and temperature (`T`). |
| `vtpdf_100_ssw.ipynb` | Generates probability distributions of wave amplitudes and phase differences at 100 hPa, 60°N. |
| `vt_amp.phase.pdf.ipynb` | Decomposes `v` and `T` into wave components and calculates amplitude and phase differences. |
| `u_z.lat.ipynb` | Analyzes zonal mean zonal wind structure as a function of height and latitude. |

---

### 📊 Key Findings

- **Topography dominates** the hemispheric asymmetry in SSWs.
- Flattening NH topography nearly eliminates SSWs in climate model simulations.
- Topography amplifies eddy heat flux by:
  - Increasing the amplitude of eddy meridional wind and temperature.
  - Decreasing their phase difference, enhancing vertical wave propagation.

---

### 🗂️ Data

The analysis uses the following datasets:

- **ECHAM6 Climate Model Simulations**  
  - ALL: Realistic topography and surface energy fluxes  
  - FLAT: Flattened topography  
  - SYMS: Symmetrized surface energy fluxes  
  - F+S: Flattened topography + symmetrized fluxes  
  - 60-year integrations with monthly and daily outputs  
  - Developed in Shaw et al. (2022)

- **ERA5 Reanalysis** (1958–2022)  
  - Zonal and meridional wind, temperature  
  - Used to evaluate model performance and calculate SSW frequency

---

### 🛠️ Environment & Dependencies

This project was developed using:

- Python 3.x
- Jupyter Notebook
- Common scientific libraries: `numpy`, `matplotlib`, `scipy`, `xarray`, `cartopy`, `netCDF4`

*Note: You may need to configure access to climate model output or reanalysis datasets used in the analysis.*

---

### 🧑‍🔬 Reproducibility

If you’d like to reproduce the analysis:

1. Clone the repository.
2. Make sure you have access to the model output files used in the simulations.
3. Run the notebooks in the order listed above, starting with `ssw_onset_dm.ipynb`.

---

### 📘 Citation

If you use this code or analysis in your work, please cite:

```
Liu, S., Shaw, T., & Garfinkel, C. I. (2025). Topography dominates the hemispheric asymmetry of stratospheric sudden warmings. Geophysical Research Letters, 52, e2024GL113051.
https://doi.org/10.1029/2024GL113051
```
