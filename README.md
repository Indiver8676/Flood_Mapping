# Flood Susceptibility, Risk and Social Vulnerability Mapping of Alappuzha District, Kerala

**Author:** Indiver Kaushik  
**Institution:** University of Calicut  
**Year:** 2026  
**Repository:** https://github.com/Indiver8676/Flood_Mapping

## 1. Project Overview

This repository contains a complete GIS- and machine learning-based flood susceptibility assessment for Alappuzha District, Kerala, India — a low-lying coastal region that is highly vulnerable to monsoon-induced compound flooding.  

A Random Forest classifier was trained using 13 conditioning factors derived primarily from SRTM 30 m DEM and other geospatial datasets. The model was validated against the 2018–2019 Kerala floods and achieved an accuracy of approximately 83% (AUC = 0.92).  

In addition to pure susceptibility mapping, the work also produced social vulnerability and integrated flood risk perspectives using Census 2011 socio-demographic indicators.

## 2. Objectives

- Develop a multi-parameter DEM-based flood susceptibility model for Alappuzha
- Train and optimise a Random Forest classifier
- Validate the model against historical flood events (2018–2019)
- Integrate social vulnerability indicators
- Provide an open and reproducible workflow

## 3. Study Area

Alappuzha District, Kerala, India. Large parts of the district lie below mean sea level and experience prolonged inundation due to heavy monsoon rainfall, tidal influence, backwater effects, and restricted drainage. The district was severely affected during the 2018 and 2019 Kerala floods.

## 4. Data and Conditioning Factors (13 Parameters)

The model used the following conditioning factors (derived mainly from SRTM 30 m DEM and complementary datasets):

1. Releif
2. Slope  
3. Curvature
4. Topographic Wetness Index (TWI)  
5. Drainage Density  
6. Distance to Rivers  
7. Land Use / Land Cover  
8. Geomorphology  
9. Rainfall  
10. NDVI  
11. Topographic Position Index (TPI)
12. Stream Power Index (SPI)
13. Convergence Index

## 5. Methodology

- Generation of conditioning factor rasters using QGIS and Google Earth Engine  
- Multicollinearity analysis  
- Training and testing data preparation  
- Random Forest classification with hyperparameter tuning  
- Accuracy assessment (Confusion Matrix, Overall Accuracy, AUC-ROC)  
- Production of a five-class flood susceptibility map  
- Integration with social vulnerability indicators from Census 2011

## 6. Key Results

- Overall Accuracy: ≈ 83%  
- AUC-ROC: 0.92  
- Final output: Five-class flood susceptibility map (Very High – Very Low)  
- Social vulnerability and integrated risk perspectives were also generated

## 7. Limitations

The 30 m resolution of the SRTM DEM was the main limitation, as it could not fully capture micro-topographic variations that influence flooding in this low-lying terrain. This limitation directly motivated subsequent work using UAV-derived high-resolution DEM and HEC-RAS 2D hydrodynamic modelling at the North Eastern Space Applications Centre (NESAC).

## 8. Repository Contents

- Jupyter notebooks covering the full workflow (data preparation, multicollinearity, model training, hyperparameter tuning, and mapping)
- Output maps and accuracy figures
- This README

## 9. How to Use

1. Clone the repository  
2. Open the notebooks in order  
3. Follow the workflow from data preparation to final model

## 10. Citation

If you use this work, please cite:

Kaushik, I. (2026). Flood Susceptibility Mapping of Alappuzha District, Kerala using Random Forest and Multi-Parameter DEM Analysis. GitHub repository. https://github.com/Indiver8676/Flood_Mapping

## 11. Contact

Indiver Kaushik  
Email: indiver.geo@gmail.com
