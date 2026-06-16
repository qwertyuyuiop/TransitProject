# TransitProject
Transit Capital Investment and Commute Mode Choice  This repository contains a reproducible R workflow analyzing how federal transit capital investments influence commute mode choice across 30+ U.S. cities. The project integrates FTA investment data with ACS commute mode data to construct a multi-year panel dataset   
## Project Structure
├─ data_raw/        # Original datasets (not uploaded)
├─ data_clean/      # Cleaned datasets or samples
├─ code/
│  ├─ 01_import.R
│  ├─ 02_clean.R
│  ├─ 03_panel.R
│  ├─ 04_regressions.R
│  ├─ 05_figures.R
│  └─ 06_export.R
├─ output/
│  ├─ figures/
│  └─ tables/
└─ docs/
   ├─ poster/
   └─ notes/

## Methods
- Data cleaning and wrangling using **tidyverse**
- Panel construction using ACS + FTA datasets
- Two-way fixed effects estimation using **fixest**
- Visualization using **ggplot2**
- Reproducible workflow using R scripts and GitHub version control

## Skills Demonstrated
- Longitudinal dataset construction  
- Fixed effects regression  
- Reproducible workflows  
- Data visualization  
- GitHub version control  

## Outputs
- Regression tables (output/tables/)
- Figures and visualizations (output/figures/)
