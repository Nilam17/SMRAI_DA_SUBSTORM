# SMRAI_DA_SUBSTORM
 SMRAI with SuperDARAN Data Assimilation for Substorm Analysis

## Data / large files (SMRAI2 and SMRAI2.1 folder)
The large dataset (~103 MB) is hosted on Zenodo (GitHub has file-size limits).

- Zenodo record (DOI): https://doi.org/10.5281/zenodo.18193241
- Direct download: https://zenodo.org/records/18193241

  
## predict_al_au_figure2.ipynb

* Downloads OMNI solar wind data for specified time ranges (You can select date 20231030 or 20231031)
* Employs SMRAI2 models (modelp099_250.sav and modelw099_300.sav) to predict electric potential and Hall conductivity
* Uploads the eletric field files for the SMRAI2.1 w/ and w/o DA methods
* Interpolates conductivity fields from SMRAI2 grid onto the SMRAI2.1 spatial grid for comparison
* Computes AL/AU indices from derived Hall currents in the auroral zone (60-70° latitude band)
* Evaluates three different AL/AU series:
  * SMRAI2 model predictions
  * SMRAI2.1 control runs (without data assimilation)
  * SMRAI2.1 with SuperDARN data assimilation (SMRAI2.1_DAssim)
* Generates time series comparison plots visualizing the performance of each approach


## all_para_plot_figure4.ipynb

* Generates detailed spatial visualization plots at selected time intervals (You can change time and date)
* Creates multi-panel polar plots displaying ionospheric potential fields (For SMRAI2. SMRAI2.1, SMRAI2.1 w/ SuperDARN DA), conductivity distributions, field-aligned current (FAC) patterns, and SuperDARN observational coverage
* Enables visual inspection of model outputs and their spatial relationships during specific substorm phases
