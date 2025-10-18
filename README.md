# Yield Curve Analysis and Forecasting

## Overview
This project focuses on the dynamic analysis and forecasting of yield curves using Principal Component Analysis (PCA) and Autoregressive (AR) models. The aim is to understand the behavior of yield curves over time, predict future movements, and perform stress testing to assess the robustness of the models.

## Data Collection
The yield curve data is sourced from the European Central Bank (ECB):  
[Euro Area Yield Curves](https://www.ecb.europa.eu/stats/financial_markets_and_interest_rates/euro_area_yield_curves/html/index.en.html)

## Methodology

### Principal Component Analysis (PCA)
PCA is used to reduce the dimensionality of the yield curve data, identifying the main factors that explain the variance in the data. This helps in simplifying the complexity and capturing the essential patterns.

### Autoregressive (AR) Modeling
AR models are applied to the principal components obtained from PCA to predict future yield curves. This involves fitting AR models to the time series data and making forecasts based on the past values.

### Visualization
The project includes various visualizations to depict the yield curves, their dynamic behavior, and the results of the forecasting models. These visualizations are created using libraries such as Matplotlib and Seaborn.

### Volatility and Stress Testing
Volatility analysis and stress testing are performed to assess the robustness of the models under different economic scenarios. This involves calculating rolling volatility and applying stress scenarios to the principal components.

## Results
- Predictions of future yield curves.
- Performance evaluation of the models using RMSE.
- Comparison with benchmark models.

## Installation and Usage
### Prerequisites
Ensure you have the following installed:
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Statsmodels

### Running the Project
1. Clone the repository:
   ```sh
   git clone https://github.com/rohank170403/Yield-Curve-Analysis-and-Forecasting.git
   cd Yield-Curve-Analysis-and-Forecasting
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the analysis scripts:
   ```sh
   python Code/analyze_yield_curve.py
   ```

## Project Structure
```
Yield-Curve-Analysis-and-Forecasting/
│-- Data/                # Contains raw and processed yield curve data
│-- Code/             # Contains Python scripts for PCA, AR models, and visualization
│-- README.md            # Project documentation
```

## Repository
[GitHub Repository](https://github.com/rishabhhshahh/Yield-Curve-Analysis-and-Forecasting)
