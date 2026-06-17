# Long-Term NDVI Trend Analysis and Forecasting for Aligarh District, Uttar Pradesh Using MODIS Satellite Data, Google Earth Engine, and Bayesian Time-Series Modelling

## Overview

This repository contains the complete research workflow, datasets, R scripts, and supporting materials developed for the M.Sc. Statistics dissertation submitted to the Department of Statistics and Operations Research, Aligarh Muslim University (AMU), Aligarh.

The study investigates long-term vegetation dynamics in Aligarh District, Uttar Pradesh, using MODIS satellite-derived NDVI data extracted through Google Earth Engine (GEE). Statistical analysis was performed in R using classical, non-parametric, time-series, and Bayesian modelling approaches.

## Dissertation Information

**Author:** MD INTJAR

**Programme:** M.Sc. Statistics

**Institution:** Department of Statistics and Operations Research, Aligarh Muslim University (AMU), India

**Academic Year:** 2025–2026

**Session:** 2025–2027

**Supervisors:**
- Dr. Haseeb Athar (Associate Professor)
- Dr. Ahmadur Rahman (Assistant Professor)

## Research Objectives

1. Analyse long-term annual and monthly NDVI trends in Aligarh District.
2. Identify seasonal vegetation patterns using monthly NDVI observations.
3. Apply statistical and time-series models for forecasting future vegetation conditions.
4. Quantify trend magnitude using classical and non-parametric methods.
5. Assess uncertainty using Bayesian linear regression.
6. Validate forecasts using an independent 2025 NDVI dataset.

## Study Area

The study focuses on Aligarh District, Uttar Pradesh, India, located in the upper Gangetic Plain. The district is characterised by intensive agricultural activity, extensive groundwater-based irrigation, and a predominance of wheat, paddy, and sugarcane cultivation.

The region was selected because of its agricultural significance and the absence of a long-term district-level NDVI dataset and forecasting framework prior to this study.

## Data Sources

### Satellite Data
- MODIS MOD13Q1 Vegetation Indices Product
- Spatial Resolution: 250 m
- Temporal Resolution: 16-day composite
- Data Period: 2001–2025
- Provider: NASA LP DAAC

### Administrative Boundary Data
- GADM Version 4.1
- Level-2 Administrative Boundary
- Study Unit: Aligarh District

### Validation Dataset
- Independently extracted monthly NDVI observations for 2025
- Used exclusively for out-of-sample forecast validation

## Software and Platforms

| Software | Purpose |
|-----------|----------|
| Google Earth Engine | NDVI extraction and preprocessing |
| R (Version 4.3.1) | Statistical analysis and modelling |
| RStudio | Code execution and project management |
| QGIS | Spatial verification and GIS operations |
| Microsoft Word | Dissertation preparation |

## Research Workflow

1. Extraction of NDVI data using Google Earth Engine.
2. Spatial verification of district boundary using QGIS.
3. Creation of annual and monthly NDVI datasets.
4. Descriptive statistical analysis.
5. Trend analysis using OLS, Mann-Kendall, and Sen's Slope.
6. Stationarity assessment using ADF, PP, and KPSS tests.
7. Time-series forecasting using ARIMA and SARIMA models.
8. Bayesian linear regression and uncertainty assessment.
9. Validation using independent 2025 NDVI observations.
10. Interpretation and synthesis of findings.

## Repository Structure

```text
ndvi-vegetation-dynamics-aligarh/
│
├── data/
│   ├── yearly_ndvi_2001_2024.csv
│   ├── monthly_ndvi_2001_2024.csv
│   ├── yearly_zonal_stats_2001_2024.csv
│   ├── monthly_zonal_stats_2001_2024.csv
│   └── validation_2025_monthly_ndvi.csv
│
├── scripts/
│   ├── yearly_analysis.R
│   ├── monthly_analysis.R
│   ├── forecasting_models.R
│   └── bayesian_analysis.R
│
├── figures/
│   ├── Figure4_1_Annual_NDVI_Trend.png
│   ├── Figure4_5_ARIMA_Forecast.png
│   ├── Figure5_1_Monthly_Heatmap.png
│   └── ...
│
├── dissertation/
│   └── MSc_Dissertation.pdf
│
└── README.md
```

## Statistical Methods

### Trend Analysis
- Ordinary Least Squares (OLS) Regression
- Mann–Kendall Trend Test
- Sen's Slope Estimator

### Stationarity Testing
- Augmented Dickey-Fuller (ADF) Test
- Phillips-Perron (PP) Test
- KPSS Test

### Time-Series Forecasting
- ARIMA Models
- Seasonal ARIMA (SARIMA)

### Bayesian Modelling
- Bayesian Linear Regression
- Posterior Predictive Analysis
- MCMC Diagnostics

## Key Findings

- Annual NDVI showed a significant positive long-term trend from 2001–2024.
- Mann-Kendall and Sen's Slope analyses confirmed vegetation improvement.
- Monthly NDVI displayed strong seasonal behaviour linked to agricultural cycles.
- ARIMA/SARIMA models successfully captured temporal dynamics.
- Validation using observed 2025 NDVI demonstrated satisfactory forecasting performance.
- Bayesian modelling provided uncertainty estimates and probabilistic interpretation of future vegetation conditions.

## Figures Generated

### Chapter 4
- Figure 4.1 Annual NDVI Trend
- Figure 4.2 Regression Diagnostics
- Figure 4.3 Sen's Slope Trend
- Figure 4.4 ACF and PACF Analysis
- Figure 4.5 ARIMA Forecast
- Figure 4.6 Yearly Validation
- Figure 4.7 Monthly NDVI Time Series
- Figure 4.8 Monthly Seasonal Pattern
- Figure 4.9 STL Decomposition
- Figure 4.10 Monthly Forecast vs Actual
- Figure 4.11 Validation Scatter Plot
- Figure 4.12 Residual Diagnostics

### Chapter 5
- Figure 5.1 Monthly NDVI Heatmap
- Figure 5.2 MCMC Trace Plot
- Figure 5.3 Posterior Density Plot
- Figure 5.4 Posterior Predictive Check
- Figure 5.5 Zonal Statistics Summary

## Citation

If you use this repository or methodology in academic work, please cite:

**Md Intjar (2026). Long-Term NDVI Trend Analysis and Forecasting for Aligarh District, Uttar Pradesh Using MODIS Satellite Data, Google Earth Engine, and Bayesian Time-Series Modelling. M.Sc. Statistics Dissertation, Aligarh Muslim University.**

## Contact

**MD INTJAR**

M.Sc. Statistics, Aligarh Muslim University

LinkedIn:
https://www.linkedin.com/in/md-intjar-statistics

Email:
intjar.bstats@gmail.com

---
© 2026 MD INTJAR. Academic and research use permitted with proper citation.
