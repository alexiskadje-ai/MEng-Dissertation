# Maize Yield Prediction using Multi-Source Data Integration

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Machine Learning](https://img.shields.io/badge/ML-XGBoost%2C%20ConvLSTM-orange)
![License](https://img.shields.io/badge/License-MIT-green)

 Overview

This repository contains the complete implementation of my Master's dissertation: "PREDICTIVE ANALYTICS FOR CROP YIELD MODELLING CASE OF MAIZE IN THE WESTERN HIGHLANDS OF CAMEROON". The research develops a hybrid machine learning framework that integrates multi-source geospatial and agricultural data to predict maize yields with uncertainty quantification.
 Research Objectives

- Develop a hybrid ConvLSTM-XGBoost model for spatio-temporal yield prediction
- Integrate heterogeneous data sources (satellite, climate, soil, yield records)
- Quantify prediction uncertainty and model interpretability
- Identify key yield determinants in the Western Highlands agro-ecological zone
- Deploy an interpretable framework for agricultural decision support

 System Architecture

![System Architecture](dissertation/figures/system_architecture.png)

The hybrid architecture combines:
- ConvLSTM: For spatio-temporal patterns from satellite time-series
- XGBoost: For tabular features from climate and soil data
- Attention-based Fusion: For optimal feature combination
- Uncertainty Quantification: Bayesian methods for prediction confidence

 Dataset Description

| Data Source | Parameters | Resolution | Period |
|-------------|------------|------------|---------|
| Satellite Imagery | NDVI, EVI, LST indices | 10-30m | 2020-2024 |
| Climate Data | Rainfall, Temperature, Humidity, Solar Radiation | Daily | 2018-2024 |
| Soil Properties | pH, N, P, K, Organic Matter | 120 sites | 2020-2024 |
| Yield Records | Maize production statistics | Regional | 2018-2024 |

 Data Sources
- Satellite: Sentinel-2 (10m), Landsat 8 (30m)
- Climate: NASA POWER, Ground Weather Stations
- Soil: Laboratory measurements from 120 sampling sites
- Yield: MINADER official statistics + 45 farm ground-truth records

 Installation & Setup

 Prerequisites
- Python 3.8+
- Jupyter Notebook
- LaTeX (for dissertation compilation)

 Installation

1. Clone the repository
bash
git clone https://github.com/yourusername/MEng-Dissertation-Maize-Yield-Prediction.git
cd MEng-Dissertation-Maize-Yield-Prediction
