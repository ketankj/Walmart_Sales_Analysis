# Walmart Sales Data Analysis

This repository contains a comprehensive analysis of Walmart's weekly sales data from 2010 to 2012 using the PACE (Plan, Analyze, Construct, Execute) framework. The analysis covers data preprocessing, exploratory data analysis (EDA), statistical testing, regression and forecasting, and additional insights such as store segmentation and feature importance.

## Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Methodology](#methodology)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Future Scope](#future-scope)
- [License](#license)

## Overview
This project aims to:
- Clean and preprocess Walmart's sales dataset.
- Visualize key trends including seasonality, holiday effects, and economic influences.
- Perform hypothesis testing to understand the impact of holidays and unemployment on sales.
- Develop regression models to predict weekly sales using factors like Fuel Price, CPI, Unemployment, and Temperature.
- Forecast future trends in fuel prices and overall sales using ARIMA and SARIMAX models.
- Segment stores using K-Means clustering and assess feature importance using Random Forest.

## Data
The dataset includes the following columns:
- **Store** (int): Store ID.
- **Date** (string): Date of the sales entry (converted to datetime).
- **Weekly_Sales** (float): Weekly sales amount.
- **Holiday_Flag** (int): Indicates if the week is a holiday (1) or not (0).
- **Temperature** (float): Temperature at the store's location.
- **Fuel_Price** (float): Price of fuel in the region.
- **CPI** (float): Consumer Price Index for the area.
- **Unemployment** (float): Unemployment rate in the area.

## Methodology
The analysis is structured using the PACE framework:
1. **Data Preprocessing & Quality Check:**  
   - Loading the CSV, checking for missing values, and converting data types.
2. **Exploratory Data Analysis (EDA):**  
   - Summary statistics, time-series visualizations, and correlation analysis.
3. **Statistical Analysis:**  
   - Hypothesis testing for holiday effects and unemployment impact on sales.
4. **Regression Analysis:**  
   - Building Linear, Ridge, and Lasso regression models.
5. **Forecasting Analysis:**  
   - Forecasting fuel prices with ARIMA and total sales with SARIMAX.
6. **Additional Insights:**  
   - Store segmentation using K-Means and feature importance with Random Forest.

## Usage
### Clone the Repository
```bash
git clone https://github.com/yourusername/walmart-sales-analysis.git
cd walmart-sales-analysis
```

### Install Dependencies
Create a virtual environment (optional) and install required libraries:
```bash
pip install -r requirements.txt
```
Example `requirements.txt`:
```txt
pandas
numpy
matplotlib
seaborn
scipy
scikit-learn
statsmodels
```

### Run the Jupyter Notebook
Launch Jupyter Notebook and open the analysis file:
```bash
jupyter notebook Walmart_Sales_Analysis.ipynb
```

### Explore the Analysis
Step through each cell to see data preprocessing, visualizations, statistical tests, model training, forecasting, and additional insights.

## File Structure
```bash
walmart-sales-analysis/
├── README.md                # This file
├── Walmart_Sales.csv        # Dataset file (if permissible to share)
├── Walmart_Sales_Analysis.ipynb  # Jupyter Notebook with full analysis
├── requirements.txt         # Python dependencies
└── images/                  # Folder for saving visualization outputs (if any)
```

## Dependencies
- Python 3.6+
- pandas
- numpy
- matplotlib
- seaborn
- scipy
- scikit-learn
- statsmodels

## Future Scope
### Feature Enhancement:
- Integrate additional store-specific features (e.g., store size, local demographics) and marketing data.

### Advanced Forecasting:
- Utilize advanced models like Prophet or LSTM for better seasonal forecasting, especially during holiday peaks.

### Granular Analysis:
- Analyze daily sales data (if available) for more detailed insights.

### Causal Inference:
- Implement causal analysis methods (e.g., Difference-in-Differences) to better understand the impact of macroeconomic changes on sales.

## License
This project is licensed under the MIT License.

## Acknowledgements
- Thanks to the creators of the libraries and tools used in this project.
- Inspiration and ideas drawn from various data analysis and forecasting tutorials.
