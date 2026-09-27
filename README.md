# 🌱 Global Sugarcane Production Analysis

> **An exploratory data analytics project analyzing sugarcane production, cultivated area, yield, and production distribution across countries and continents using Python.**

![Python](https://img.shields.io/badge/Python-Data%20Analysis-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557c)
![Seaborn](https://img.shields.io/badge/Seaborn-EDA-4c9c8c)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter)

---

## 🌎 Project Overview

The **Global Sugarcane Production Analysis** project explores the worldwide distribution of sugarcane production using country-level agricultural data.

The analysis focuses on four major dimensions:

* 🌱 Total sugarcane production
* 🌾 Cultivated acreage
* 📈 Yield per hectare
* 👥 Production per person

The project uses Python-based exploratory data analysis to understand:

* Which countries produce the most sugarcane?
* Which continents dominate production?
* Does cultivated land influence total production?
* How does yield vary across countries?
* What is the production contribution of individual countries?
* What relationships exist between agricultural variables?

The repository contains a **103-country dataset** and a detailed Jupyter Notebook implementing the analysis.

---

# 🎯 Analytical Objectives

The project investigates the following business and agricultural questions:

### 🌍 1. Country-Level Production

Identify the countries with the highest sugarcane production.

### 🌾 2. Land Utilization

Analyze the relationship between cultivated acreage and total production.

### 📈 3. Yield Analysis

Compare sugarcane yield across countries.

### 👥 4. Production Per Person

Analyze production relative to population-related measures in the dataset.

### 🌎 5. Continental Distribution

Determine how production is distributed across continents.

### 📊 6. Production Contribution

Calculate the percentage contribution of countries to overall sugarcane production.

### 🔗 7. Correlation Analysis

Investigate relationships between:

* Production
* Acreage
* Yield
* Production per person

---

# 📊 Dataset

### Dataset Structure

| Metric                | Description                     |
| --------------------- | ------------------------------- |
| Country               | Country name                    |
| Continent             | Geographic continent            |
| Production (Tons)     | Total sugarcane production      |
| Production per Person | Sugarcane production per person |
| Acreage (Hectare)     | Land used for production        |
| Yield (Kg / Hectare)  | Production efficiency           |

The original dataset contains **103 country-level observations and 7 columns**, including an index column. The notebook performs data cleaning and reduces the analytical structure for subsequent analysis.

---

# 🔄 Data Analytics Workflow

```text
              RAW AGRICULTURAL DATA
                       │
                       ▼
                Data Inspection
                       │
                       ▼
              Data Type Conversion
                       │
                       ▼
                 Data Cleaning
                       │
                       ▼
            Missing Value Analysis
                       │
                       ▼
           Exploratory Data Analysis
                       │
              ┌────────┼────────┐
              ▼        ▼        ▼
          Country   Continent  Correlation
          Analysis   Analysis    Analysis
              │        │        │
              └────────┼────────┘
                       ▼
               Business Insights
```

---

# 🧹 Data Cleaning

The original dataset contains formatted numeric values using separators such as periods and commas.

The notebook standardizes these values before numerical analysis.

### Cleaning Operations

* Convert formatted production values
* Standardize decimal notation
* Convert agricultural metrics into numerical types
* Rename columns for easier analysis
* Check missing values
* Remove unnecessary indexing information
* Prepare the dataset for statistical analysis

The notebook identifies missing values in acreage and yield for one observation before subsequent analysis.

---

# 🐍 Python Analysis

The project is implemented using:

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### Main Libraries

| Library    | Purpose                   |
| ---------- | ------------------------- |
| Pandas     | Data manipulation         |
| NumPy      | Numerical analysis        |
| Matplotlib | Visualization             |
| Seaborn    | Statistical visualization |
| Jupyter    | Interactive analysis      |

---

# 🏆 Country-Level Production

The analysis identifies major sugarcane-producing countries.

The dataset shows:

| Country       |   Production |
| ------------- | -----------: |
| 🇧🇷 Brazil   | ~768.7M tons |
| 🇮🇳 India    | ~348.4M tons |
| 🇨🇳 China    | ~123.1M tons |
| 🇹🇭 Thailand |  ~87.5M tons |
| 🇵🇰 Pakistan |  ~65.5M tons |

These values come directly from the repository's dataset/notebook output.

---

# 📈 Production Contribution

The notebook calculates each country's contribution to total production.

The analysis shows that Brazil accounts for approximately **40.7%** of the production represented in the dataset, while India contributes approximately **18.5%**.

This provides a useful way to move beyond absolute production and understand **relative contribution to global production within the dataset**.

---

# 🔗 Correlation Analysis

A correlation matrix is used to investigate relationships between agricultural variables.

One of the strongest relationships identified is:

### Production ↔ Acreage

**Correlation ≈ 0.99755**

This indicates a very strong positive linear relationship between cultivated acreage and total production in this dataset.

The project also visualizes the correlation matrix using a Seaborn heatmap.

### Important Interpretation

Correlation does **not** by itself prove causation.

The result indicates that countries with greater cultivated acreage tend to have greater total production within this dataset; it does not establish that acreage alone causes higher production.

---

# 🌾 Acreage vs Production Analysis

The project specifically investigates the question:

> **Does a country with more cultivated land produce more sugarcane?**

A scatter-based analysis is used to explore the relationship between:

```text
Acreage (Hectare)
        ↓
Production (Tons)
```

This analysis complements the correlation matrix and provides a visual interpretation of the relationship.

---

# 🌎 Continental Analysis

The project aggregates agricultural metrics by continent to compare regional production patterns.

The analysis examines:

* Total production
* Average production-related metrics
* Number of countries
* Geographic distribution

The notebook also creates continent-level visualizations to identify the dominant production regions.

---

# 📊 Key Analytical Insights

### 🥇 Production Concentration

Brazil represents the largest production value in the dataset, followed by India, China, Thailand, and Pakistan.

### 🌾 Land and Production

Production and cultivated acreage have an extremely strong positive correlation of approximately **0.99755** in the analyzed dataset.

### 🌍 Geographic Distribution

The dataset enables production comparison across Africa, Asia, Europe, North America, Oceania, and South America.

### 📊 Production Concentration

The country-level production-share analysis highlights how a relatively small number of major producers account for a substantial portion of the dataset's total production.

---

# 📁 Repository Structure

```text
Sugarcane-Production/
│
├── List of Countries by Sugarcane Production.csv
│       └── Country-level agricultural dataset
│
├── SugarCane Production Project.ipynb
│       └── Complete Python EDA
│
├── Sugarcane Product Project .pdf
│       └── Project documentation
│
├── vertopal.com_SugarCane Production Project.pdf
│       └── PDF project export
│
└── README.md
```

The current repository contains these four project assets besides the README.

---

# 🧠 Skills Demonstrated

## Data Analytics

* Exploratory Data Analysis
* Data Cleaning
* Missing Value Analysis
* Numerical Data Transformation
* Descriptive Analysis
* Aggregation
* Ranking
* Percentage Contribution Analysis

## Statistical Analysis

* Correlation Analysis
* Correlation Matrix
* Relationship Analysis
* Distribution Analysis

## Data Visualization

* Bar Charts
* Scatter Plots
* Heatmaps
* Country-Level Comparisons
* Continental Comparisons

## Python

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

# 🚀 How to Run

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Sugarcane-Production
```

## 2. Install Dependencies

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## 3. Launch Jupyter

```bash
jupyter notebook
```

Open:

```text
SugarCane Production Project.ipynb
```

## 4. Load the Dataset

Make sure:

```text
List of Countries by Sugarcane Production.csv
```

is available in the working directory, then update the notebook's CSV path if necessary.

---

# 🔬 Future Improvements

The project can be extended into a more advanced agricultural analytics solution.

### Predictive Analytics

* Sugarcane production forecasting
* Yield prediction
* Production trend modeling

### Machine Learning

* Regression models for production prediction
* Feature importance analysis
* Country-level clustering
* Yield classification

### Geographic Analytics

* Choropleth maps
* Country-level geographic visualization
* Regional production dashboards

### Advanced Agricultural Analytics

* Production efficiency score
* Acreage utilization analysis
* Yield benchmarking
* Production-per-hectare optimization
* Country benchmarking

### Business Intelligence

A Power BI dashboard could be added containing:

* Global production KPIs
* Top producer rankings
* Production by continent
* Acreage vs production
* Yield comparison
* Country contribution
* Interactive country filters

---

# 📌 Project Takeaway

This project demonstrates how a relatively simple agricultural dataset can be transformed into a structured analytical study by combining:

> **Data Cleaning → Exploratory Analysis → Statistical Relationships → Geographic Comparison → Business Insights**

The project is particularly useful for demonstrating practical Python-based analytics, statistical reasoning, data visualization, and the ability to convert raw agricultural data into interpretable findings.

---

# 👤 Author

**Aryan Mishra**

B.Tech CSE | Data Analyst | Python | SQL | Power BI | Machine Learning

Email: [aryanmishra01718@gmail.com](mailto:aryanmishra01718@gmail.com)

---
