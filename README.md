# GEOG5990M-Final-Assignment
# Spatial Analysis of Commuting Distance in Leeds

## 1. Project Overview
This project investigates how average commuting distance varies across Lower Layer Super Output Areas (LSOAs) in Leeds.  
The analysis uses open data from the 2021 Census (Nomis) and LSOA boundary data from the ONS Geoportal.  
All processing, analysis, and visualisation are conducted in Python using GeoPandas.

---

## 2. Data in This Repository
This repository includes all files required to reproduce the analysis:

- **LSOA_Leeds.geojson**  
  Subset of the national 2021 LSOA boundary dataset, filtered to Leeds only.

- **leeds_commuting_distance.csv**  
  Cleaned commuting distance data with grouped distance categories.

- **project.ipynb**  
  Notebook containing all data cleaning, feature engineering, spatial joins, modelling, and visualisation.

**Not included:**  
- Full national LSOA dataset (>25MB).  
  This is stored in Google Drive and loaded directly in the notebook.

---

## 3. What the Notebook Does
- Loads LSOA boundaries and filters to Leeds  
- Cleans commuting distance data  
- Converts grouped distance categories into a weighted average commuting distance  
- Merges census data with spatial boundaries  
- Produces statistical summaries and visualisations  
- Fits a simple OLS model exploring spatial patterns  
- Generates a choropleth map of commuting distance across Leeds

---

## 4. How to Reproduce the Analysis

### Google Colab 
1. Open the notebook in Colab  
2. Mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')

##5.Repository Structure
GEOG5990M-Final-Assignment/
│
├── data/
│   ├── LSOA_Leeds.geojson
│   └── leeds_commuting_distance.csv
│
├── analysis.ipynb
└── README.md

##7. Reproducibility
Running the notebook from start to finish will reproduce all data processing, analysis, modelling, and visualisations presented in the final report.
##8. References
Brewer (1999); Few (2012); Longley et al. (2015); ONS (2021); Slocum et al. (2009).

