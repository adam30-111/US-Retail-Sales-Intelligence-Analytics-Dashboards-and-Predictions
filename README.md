# 🛒 US Retail Sales Intelligence Analytics Dashboards and Predictions

> **End-to-end data analytics project** exploring 4 years of US retail superstore data — from data cleaning and EDA to interactive dashboards and machine learning predictions.

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-✓-150458.svg)
![Plotly](https://img.shields.io/badge/Plotly-✓-3F4F75.svg)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-✓-F7931E.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)

---

## 📊 Project Overview

This project analyzes a US retail superstore dataset spanning **2015–2018**, covering **9,789 transactions**, **793 customers**, and **48 states**. The goal is to uncover sales drivers, customer behavior, geographic trends, and shipping performance, then translate those findings into business-actionable strategies.

The project is structured around three deliverables: a deep exploratory analysis, an interactive dashboard, and a final insights report with an ML prediction model.

---

## 🎯 Key Findings

- 💰 **2.25 million dollars** in total revenue across 4,916 unique orders, with **+50 percent net growth** from 2015 to 2018
- 🏆 **California alone drives 20 percent** of total sales; the top 3 states generate approximately 41 percent
- 📦 **Technology category** leads revenue at 37 percent despite having the lowest order count
- ⚠️ **The Outlier Paradox:** 12 percent of orders generate **64 percent of total revenue** — these are not errors, they are the business
- 👥 **Zero overlap** between top customers by frequency and top customers by lifetime value — two distinct segments
- 🚚 **Same Day shipping** under-utilized at only 5.5 percent — clear premium upsell opportunity
- 📅 **November is the peak month** every single year, driven by holiday shopping

---

## 🗂️ Repository Structure

```
US-Retail-Sales-Intelligence-Analytics-Dashboards-and-Predictions/
├── data/
│   ├── Sales_cleaned_data.csv      # Cleaned & feature-engineered
│   └── Sales_raw_data.csv          # Original dataset
├── images/                         # Screenshots & visualizations 
├── notebooks/
│   ├── 01_EDA.ipynb                # Exploratory Data Analysis
│   ├── 02_Dashboard.ipynb          # Interactive Plotly Dashboard
│   └── 03_Insights_and_ML.ipynb    # Key Insights + ML Model                       
├── README.md
└── requirements.txt
```

---

## 📓 Notebooks

### 1️⃣ Exploratory Data Analysis

A comprehensive EDA covering:

- **Data Cleaning** — Handling missing values, type conversion, duplicates check
- **Feature Engineering** — Date components, shipping duration
- **Univariate Analysis** — Sales distribution, log-normal pattern identification
- **Geographic Analysis** — State-level and regional breakdowns
- **Product Analysis** — Category, sub-category, and product-level insights
- **Temporal Analysis** — Year-over-year growth and seasonality heatmaps
- **Outlier Investigation** — IQR-based detection and business interpretation

### 2️⃣ Interactive Dashboard

A Plotly-based dashboard featuring:

- 📊 **8 KPI cards** with key business metrics
- 📈 **Monthly sales trends** with annotations
- 🗺️ **USA choropleth map** showing state-level performance
- 🛒 **Category and sub-category breakdowns**
- 🚚 **Shipping mode analysis** by state and duration
- 💡 **Insights summary** translating numbers into recommendations

### 3️⃣ Insights & ML Model

The final deliverable combining:

- **🔍 Key Insights Summary** — Business performance, top performers, customer insights
- **⚠️ Notable Anomalies** — The Outlier Paradox, Frequency-Value disconnect, volume-revenue inversion
- **🎯 Strategic Recommendations** — 8 actionable business strategies
- **🤖 ML Prediction Model** — Three-model comparison (Linear Regression, Random Forest, Gradient Boosting) with log-transformation, feature importance analysis, and sample predictions

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Python 3.10** | Core programming language |
| **Pandas, NumPy** | Data manipulation and analysis |
| **Matplotlib, Seaborn** | Static visualizations |
| **Plotly** | Interactive dashboards and charts |
| **Scikit-learn** | Machine learning models |
| **Jupyter / Google Colab** | Notebook environment |

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install -r requirements.txt
```

### Run the notebooks

```bash
# Option 1: Local Jupyter
jupyter notebook

# Option 2: Open directly in Google Colab
# Click any notebook in the notebooks/ folder and select "Open in Colab"
```

---

## 📈 ML Model Performance

| Model | R² (log scale) | MAE |
|-------|----------------|-----|
| Linear Regression | 0.42 | $194 |
| Random Forest | 0.31 | $207 |
| Gradient Boosting | 0.41 | $194 |

**Key insight:** Applying a log transformation to the heavily skewed Sales column improved model performance from **R² ≈ -0.002** (worse than predicting the mean) to **R² ≈ 0.40** — a dramatic improvement. The strongest predictors are **product Category** and **Sub-Category**, confirming that product type is the primary driver of sales value.

---

## 🎓 About This Project

This project was completed as part of the **Data Science Pathline (Level I)** certification. It demonstrates a full data analytics workflow: from raw data through cleaning, exploration, visualization, dashboarding, business insights, and machine learning.

---

## 👤 Author

**Adam Sameh** — [GitHub Profile](https://github.com/adam30-111)
