# DengAI – Predicting Disease Spread
## Competition: DengAI: Predicting Disease Spread (DrivenData)
Competition URL: [click here](https://www.drivendata.org/competitions/44/dengai-predicting-disease-spread/)
--- 

## Overview
- This project aims to predict weekly dengue fever cases in two cities — `San Juan` and `Iquitos` using environmental and climate data such as temperature, precipitation, humidity, and vegetation. The goal is to forecast the number of reported dengue cases based on past climate and environmental patterns.

--- 

## 📚 Dataset Description

- The provided dataset includes, for each week (by city, year, week-of-year): climate and environmental variables along with historical dengue case counts (for training). Features include: 
1. Temperature: max, min, average, diurnal range (°C)
2. Precipitation (from station / satellite / reanalysis data)
3. Humidity (relative, specific)
4. Dew point temperature, air temperature (from reanalysis)
5. Vegetation indices (NDVI) for multiple quadrants around each city location 
6. Target label: total_cases — the number of dengue cases reported that week (integer). 
7. Evaluation metric: Mean Absolute Error (MAE) between your predictions and actual case counts. 

--- 

## Methodology / Approach
- Data cleaning / preprocessing: Handling missing values (NaNs), type conversions, date parsing amd renamimg columns.
- Visualizations: line graph, bar graphs, heatmap, baxplot.
- Models: Random Forest Regressor / XGB Regressor / Linear Regression
- Evaluation: MAE, MSE, R2 score
- Prediction: Generating weekly case count predictions for both cities for the test set, formatting according to submission requirements: a CSV with columns city, year, weekofyear, total_cases.

---

## License / Notes

- This repository contains only the code, output and model logic. The original data is under the usage restrictions of DrivenData’s competition rules, and cannot be publicly redistributed.
