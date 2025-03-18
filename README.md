# **Walmart Sales Data Analysis**

This repository contains a **comprehensive analysis** of Walmart's **weekly sales data (2010–2012)** using the **PACE (Plan, Analyze, Construct, Execute) framework**. The project includes **SQL-based data preprocessing, Power BI visualizations, statistical modeling, forecasting, and machine learning insights**.

## 📌 Table of Contents
- [Overview](#overview)
- [Data](#data)
- [Methodology](#methodology)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Future Scope](#future-scope)
- [License](#license)

## 📊 Overview
This project aims to:
✔ **Clean and preprocess** Walmart's sales dataset using **SQL & Python**.  
✔ **Visualize key trends** using **Power BI**, including **seasonality, holiday effects, and economic influences**.  
✔ **Perform hypothesis testing** to understand the impact of **holidays and unemployment on sales**.  
✔ **Develop regression models** to predict weekly sales using factors like **Fuel Price, CPI, Unemployment, and Temperature**.  
✔ **Forecast future trends** using **ARIMA and SARIMAX models** for total sales and fuel prices.  
✔ **Segment stores using K-Means clustering** and assess **feature importance using Random Forest**.

## 📂 Data
The dataset includes:

| **Column**         | **Data Type** | **Description** |
|--------------------|--------------|----------------|
| **Store**         | Integer       | Store ID |
| **Date**          | DateTime      | Sales entry date |
| **Weekly_Sales**  | Float         | Total weekly sales per store |
| **Holiday_Flag**  | Integer (0/1) | Indicates if the week includes a holiday |
| **Temperature**   | Float         | Local temperature at the store |
| **Fuel_Price**    | Float         | Fuel price in the region |
| **CPI**          | Float         | Consumer Price Index |
| **Unemployment**  | Float         | Regional unemployment rate |

## 🔬 Methodology
The analysis follows the **PACE framework**:

### 1️⃣ Data Preprocessing & SQL Optimization
✔ **Loaded and cleaned data** using **SQL (MySQL/PostgreSQL)**.  
✔ Used **SQL Views & Indexed Tables** to optimize queries, improving report performance.

### 2️⃣ Exploratory Data Analysis (EDA) & Power BI Visualizations
✔ **Built interactive dashboards** in **Power BI** to analyze sales trends, seasonality, and regional variations.  
✔ **Analyzed correlations** between sales and economic factors (Fuel Price, CPI, Unemployment).

### 3️⃣ Statistical Analysis & Hypothesis Testing
✔ Conducted **hypothesis testing** to measure the effect of holidays and economic shifts on sales.

### 4️⃣ Regression & Machine Learning Models
✔ **Built Linear, Ridge, and Lasso Regression models** to predict weekly sales.  
✔ Used **Random Forest** to determine the **most important sales-driving factors**.

### 5️⃣ Forecasting Analysis
✔ Implemented **ARIMA & SARIMAX models** to forecast **sales and fuel price trends**.

### 6️⃣ Store Segmentation & Feature Importance
✔ **Clustered stores using K-Means** to identify performance-based store categories.

## 🛠 Usage

### Clone the Repository
```bash
git clone https://github.com/yourusername/walmart-sales-analysis.git
cd walmart-sales-analysis
```

### Run SQL Preprocessing (MySQL / PostgreSQL)
1. Import the provided **`Walmart_Sales.sql`** file into your database.
2. Run the **SQL Queries for data transformation** (Views, Indexing, Data Cleaning).
3. Export **cleaned data** into **CSV format** for further analysis.

### Install Dependencies (Python)
```bash
pip install -r requirements.txt
```

### Run Jupyter Notebook for Python Analysis
```bash
jupyter notebook Walmart_Sales_Analysis.ipynb
```

### Explore Power BI Dashboard
1. Open **`Walmart_Sales_Analysis.pbix`** in Power BI.
2. View **interactive sales dashboards & insights**.

## 📁 File Structure
```bash
walmart-sales-analysis/
├── README.md                      # Project Documentation
├── Walmart_Sales.sql               # SQL script for data processing
├── Walmart_Sales.csv               # Cleaned dataset (if permissible)
├── Walmart_Sales_Analysis.ipynb    # Jupyter Notebook with full analysis
├── Walmart_Sales_Analysis.pbix     # Power BI Report
├── requirements.txt                # Python dependencies
└── images/                         # Folder for saving visualization outputs (if any)
```

## 📈 Power BI Dashboard Sneak Peek
🔹 **Sales Trends Analysis** – Interactive visuals of **weekly sales performance**.  
🔹 **Seasonality & Holiday Impact** – Comparative analysis of **holiday vs. non-holiday weeks**.  
🔹 **Regional Sales Trends** – Fuel Price, CPI, and Unemployment **impact on store sales**.

📌 **[Add Screenshot Here]**  

## 🔮 Future Scope
✔ **Enhanced Store-Level Analysis** – Integrate **store size, demographics, marketing data**.  
✔ **Advanced Forecasting** – Implement **Prophet or LSTM models** for seasonal trend prediction.  
✔ **Granular Analysis** – Extend analysis to **daily** rather than weekly sales.  
✔ **Causal Inference** – Use **Difference-in-Differences (DID) methodology** to analyze macroeconomic impacts.

## 📜 License
This project is licensed under the **MIT License**.