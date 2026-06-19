# TransitProject
Transit Capital Investment and Commute Mode Choice  This repository contains a reproducible R workflow analyzing how federal transit capital investments influence commute mode choice across 30+ U.S. cities. The project integrates FTA investment data with ACS commute mode data to construct a multi-year panel dataset   
## Project Structure
\\\
├── data_raw/                     # Original ACS + FTA datasets (not uploaded)
│
├── data_clean/                   # Cleaned datasets used in analysis
│   ├── acs_clean.csv
│   ├── fta_clean.csv
│   ├── rail_heavy.csv
│   ├── rail_light.csv
│   ├── rail_commuter.csv
│   └── panel_city_year.csv
│
├── code/                         # Reproducible R scripts
│   ├── 01_import.R               # Load ACS + FTA data
│   ├── 02_clean.R                # Clean and standardize variables
│   ├── 03_panel.R                # Construct city-year panel dataset
│   │
│   ├── reg_1lag.R                # FE models with 1-year lag of investment
│   ├── reg_2lag.R                # FE models with 2-year lag
│   ├── reg_3lag.R                # FE models with 3-year lag
│   ├── reg_4lag.R                # FE models with 4-year lag
│   │                             # Each script includes:
│   │                             #   - Car ridership models
│   │                             #   - Heavy rail models
│   │                             #   - Light rail models
│   │                             #   - Commuter rail models
│   │
│   ├── 05_figures.R              # Trend plots + regression visualizations
│   └── 06_export.R               # Export tables and figures
│
├── output/
│   ├── tables/                   # Regression tables by lag year + mode
│   │   ├── car/
│   │   ├── rail/
│   │   
│   │   
│   │
│   └── figures/                  # Visualizations (trends + FE estimates)
│
└── docs/
    ├── poster/                   # Research poster and presentation materials
    └── notes/                    # Methodological notes and drafts
\\\

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
