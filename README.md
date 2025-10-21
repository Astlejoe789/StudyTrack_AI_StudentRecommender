# 🧠 Milestone 1 – Smart Purchase Pattern Analyzer

## 🏷️ Project Title: **AI-Based Consumer Behavior Analysis using Data-Driven Insights**

**Internship:** Infosys Springboard – _Study Track: AI-Based Student Study Habit Recommender_  
**Milestone:** 1 – Data Preprocessing and Exploratory Data Analysis (EDA)  
**Intern:** Astle Joe A S  
**Domain:** Artificial Intelligence & Machine Learning

---

## 🎯 Objective

The goal of this milestone is to demonstrate the ability to perform **data preprocessing** and **exploratory data analysis (EDA)** on two related datasets.  
The project explores **consumer purchasing patterns** to understand how demographic and behavioral features influence purchase trends.

This foundation prepares the data for advanced **machine learning tasks** like recommendation systems or predictive modeling in future milestones.

---

## 📂 Dataset Overview

Two related CSV files were selected for this milestone to ensure relational consistency and analytical depth.

| File Name              | Description                                                                            | Common Key    |
| ---------------------- | -------------------------------------------------------------------------------------- | ------------- |
| `customer_details.csv` | Contains demographic information such as Customer ID, Gender, Age, and Region.         | `Customer_ID` |
| `basket_details.csv`   | Contains transaction details such as Basket ID, Item Count, Purchase Amount, and Date. | `Customer_ID` |

These datasets were merged using the **`Customer_ID`** field to create a unified analytical dataset for exploration and visualization.

---

## 🧹 Data Preprocessing Steps

### 1️⃣ Merging Datasets

Combined `customer_details.csv` and `basket_details.csv` using **Pandas `merge()`** on `Customer_ID`.

### 2️⃣ Handling Missing Values

- Identified missing entries using `isnull()`.
- Replaced numeric nulls with **mean/median values** and categorical nulls with **mode** or defaults.

### 3️⃣ Removing Duplicates

- Applied `drop_duplicates()` to ensure unique records.

### 4️⃣ Data Type Correction

- Converted data columns to appropriate numerical, categorical, or datetime formats.

### 5️⃣ Encoding Categorical Variables

- Used **Label Encoding** on columns such as `Gender` and `Region` for consistency.

### 6️⃣ Optional Scaling/Normalization

- Standardized numerical attributes like `Purchase_Amount` and `Item_Count` for better comparability.

---

## 📈 Exploratory Data Analysis (EDA)

The EDA phase focuses on discovering **patterns, correlations, and insights** using descriptive statistics and visualizations.

### 🔍 Descriptive Analysis

- Calculated **mean, median, standard deviation**, and **correlation matrix** using `describe()` and `corr()`.
- Identified **outliers** and **data skewness** in purchase patterns.

### 📊 Visualization Summary

| Visualization Type | Description                                  |
| ------------------ | -------------------------------------------- |
| **Histogram**      | Distribution of purchase amounts             |
| **Bar Plot**       | Average purchase amount by gender            |
| **Scatter Plot**   | Relationship between age and purchase amount |
| **Heatmap**        | Correlation between numerical features       |

---

## 🧠 Key Insights

- **Gender-based Spending:** Male and female customers show distinct purchasing behaviors in average spending.
- **Age Influence:** Younger customers (below 30) tend to make higher purchase amounts compared to older age groups.
- **Regional Variation:** Certain regions show higher transaction values and purchase frequency.
- **Correlations:** Purchase amount shows moderate correlation with both age and basket size, indicating potential for predictive modeling.

---

## ⚙️ Tools & Technologies

| Category            | Tools/Packages Used                  |
| ------------------- | ------------------------------------ |
| **Data Handling**   | Python (Pandas, NumPy)               |
| **Visualization**   | Matplotlib, Seaborn                  |
| **Preprocessing**   | Scikit-learn (LabelEncoder, scaling) |
| **Environment**     | Google Colaboratory                  |
| **Version Control** | GitHub                               |

---

## 📘 Folder Structure

```
Milestone1/
├── Milestone1_EDA.ipynb # Main Colab Notebook
├── data/
│ ├── customer_details.csv # Customer dataset
│ └── basket_details.csv # Basket/transaction dataset
└── README.md # Project overview and report
```

---

## 📍 Outcomes

✅ Successfully cleaned, merged, and visualized two related datasets.  
✅ Derived meaningful business insights to support AI-based recommendation modeling.  
✅ Prepared a reproducible, well-documented notebook following professional coding standards.

---

## 🚀 Future Scope

- Develop a **Recommendation Engine** using purchase history and demographics.
- Implement **Predictive Modeling** for forecasting future purchase amounts.
- Apply **Clustering Algorithms** to segment customers based on buying behavior.

---

## 👨‍💻 Author

**Astle Joe A S**  
B.Tech Artificial Intelligence & Machine Learning (AIML)  
**Infosys Springboard Internship – Data Analytics & AI Track**  
**GitHub Portfolio:** _(https://github.com/Astlejoe789)_  
📅 **Date:** 21 October 2025
