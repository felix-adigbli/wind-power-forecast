# wind-power-forecast
## Overview
This project aims to predict wind power output at least 24 hours in advance to aid electric utility companies in planning power input requirements for electrical grids. Using the Spatial Dynamic Wind Power Forecasting (SDWPF) dataset, the project incorporates data from 134 wind turbines in a wind farm in China. The dataset includes various features such as wind speed, wind direction, temperature, and power output, enabling advanced machine learning models to forecast active power generation.

## Problem Statement
Electric utility companies require accurate wind power predictions to optimally balance energy supply from alternative sources. This project focuses on predicting the active power output (Patv) of wind turbines based on meteorological and operational parameters.

## Key Highlights
`Interactive Visualization`: Explore data relationships with widgets in Jupyter Notebook.
`Robust Feature Engineering`: Employ advanced techniques to extract maximum information.
`Scalable Models`: Designed for integration with both simple and advanced ML frameworks.


## Dataset
The SDWPF dataset contains measurements from wind turbines, including:

.`TurbID`: Turbine ID.
.`Day`: Day of the measurement (starting from May 1, 2020).
.`Tmstamp`: Timestamp of the measurement.
.`Wspd`: Wind speed (m/s).
.`Wdir`: Wind direction (°).
.`Etmp`: Environmental temperature (°C).
.`Itmp`: Internal nacelle temperature (°C).
.`Ndir`: Nacelle direction (°).
.`Pab1`, Pab2, Pab3: Blade pitch angles (°).
.`Prtv`: Reactive power (kW).
.`Patv`: Active power (kW, target variable).

## Project Highlights
### 1. Exploratory Data Analysis (EDA)
    Visualizations: Histograms, scatter plots, time series, and correlation matrices.
    Identification of missing and abnormal values.
    Distribution and relationships between features.
### 2. Data Preprocessing
    Cleaning: Removal of missing and abnormal values.
    Feature Engineering: Transformation of angle features, interpolation for temperature corrections, and generation of time-based sinusoidal features.
    Subset Selection: Analysis of top-performing turbines by energy output.
### 3. Baseline Models
    Linear Regression: Predicts active power based solely on wind speed.
    Feature Importance Analysis: Ranks predictors by their impact on performance.
### 4. Advanced Models
    Multivariate Linear Regression: Includes additional predictors such as temperature and nacelle direction.
    Neural Networks: Customizable models with three hidden layers to capture non-linear relationships.
    SHAP Analysis: Explains feature importance using SHAP values.
### 5. Interactivity
    Widgets and interactive plots for visualization.
    Adjustable parameters for turbines, features, and time ranges.
### 6. Evaluation
    Visualize results using scatter plots and feature importance scores.
    Use metrics like Mean Absolute Error (MAE) for evaluation.



## Future Enhancements
    . Integration of real-time data streams.
    . Deployment on cloud platforms for production-ready forecasting.
    . Exploring alternative machine learning models, such as XGBoost.


### Acknowledgments
SDWPF Dataset Authors
Machine Learning Frameworks: TensorFlow, PyTorch, Scikit-learn
Visualization Tools: Matplotlib, Seaborn