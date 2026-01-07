# FUTURE_ML_01
AI-Powered Rossmann Sales Forecasting with Prophet. Jupyter notebooks from an internship project: cleaned data with Pandas, engineered seasonal/holiday features, trained Prophet for time series predictions, and visualized trends via Seaborn.

# Rossmann Store Sales Forecasting 

## Project Overview
Developed as part of my **Machine Learning Internship at Future Interns (Task 1)**, this project implements a high-precision forecasting engine to predict daily sales for 1,115 Rossmann stores. 

In the 2026 retail landscape, static forecasting is insufficient. This project utilizes a **Multivariate Facebook Prophet** approach to account for complex external drivers, ensuring that predictions remain robust against market volatility.

## Technical Stack
- **Language:** Python 3.12+
- **Modeling:** [Facebook Prophet](facebook.github.io)
- **Data Wrangling:** Pandas & NumPy
- **Validation:** Prophet Diagnostics (Cross-Validation & Performance Metrics)

## Key Features
### 1. Multivariate Regressor Integration
Unlike standard univariate models, this implementation dynamically incorporates store-specific features to improve accuracy. Key regressors include:
- Promotional cycles (Promo, Promo2)
- Competition distance and entry dates
- State and School holidays
- Store-specific assortments and types

### 2. Automated Feature Engineering
I developed a programmatic workflow to iterate through store attributes and inject them as regressors into the Prophet model, allowing for a scalable and maintainable codebase.

### 3. Rigorous Cross-Validation
To ensure the model is "business-ready," I performed time-series cross-validation across multiple horizons (3 to 12 days).

## Model Performance
The model was evaluated using **RMSE**, **MAE**, and **MDAPE** to ensure stability across different prediction windows.

Rossmann Sales Model Summary:

  Best Accuracy: 7-Day Horizon (MDAPE: 12.3%)
  Average Error: MAE 1336.00
  Confidence: 78% Average Coverage across 10-day forecast period.

## Dataset
This project uses the Rossmann Store Sales Dataset. The dataset is known for its high dimensionality and the challenge of managing store-specific trends.

## Installation & Usage

### 1. Clone the repository: 
  git clone https://github.com/AnoMi-1/FUTURE_ML_01.git

### 2. Install dependencies:
 pip install -r requirements.txt

### 3. Run the Jupyter Notebook:
   jupyter notebook FUTURE_ML_01.ipynb

    
