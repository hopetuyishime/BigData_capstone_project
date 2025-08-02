# 🏡 Household Energy Consumption Analysis & Dashboard

## 📌 Introduction

The **Household Energy Consumption Analysis** project aims to analyze energy usage patterns across various households and provide actionable insights for improving energy efficiency. The dataset consists of 188 households with attributes such as dwelling type, household size, heating sources, education index, income levels, energy efficiency class, and daily energy consumption (kWh/day).

Using **Python (Machine Learning)** and **Power BI**, this project provides:

* Predictive modeling of household energy consumption
* Segmentation of households using clustering
* An interactive Power BI dashboard for visualization and decision-making

---

## 🎯 Objectives

* **Data Cleaning:** Standardize column names, handle missing values, and ensure data consistency.
* **Feature Engineering:** Convert categorical and numerical variables for model training.
* **Machine Learning:** Build a regression model to predict `kWh/day` consumption.
* **Clustering:** Segment households based on energy usage patterns.
* **Visualization:** Create a Power BI dashboard to communicate insights clearly.
* **Innovation:** Enhance predictions using ensemble techniques and provide interactive analytics.

---

## 📂 Dataset Overview

* **Total Rows:** 188 households
* **Total Features:** 38 columns
* **Key Columns:**

  * **House Characteristics:** `dwelling`, `dwelling_grade`, `household_m2`, `bedrooms`, `heating_source`
  * **Demographics:** `occupants`, `children`, `teenagers`, `adults`, `elders`
  * **Socioeconomic:** `income`, `education_index`, `recycling`, `awareness`
  * **Energy Metrics:** `energy_class`, `thermostats`, `smart_plugs`, `water_heater`, `kwh/day`, `hdd`, `cdd`
  * **Time Metrics:** `start`, `end`, `days`

---

## 🔧 Data Cleaning & Preprocessing

1. **Normalized column names** for consistency
2. **Removed empty rows** and placeholder headers
3. **Handled missing values** via imputation or row removal
4. **Converted income strings to numeric values**
5. **Encoded categorical variables** for machine learning models
6. **Standardized numeric features** using `StandardScaler`

---

## 🤖 Machine Learning Implementation

* **Model Used:** `RandomForestRegressor`
* **Features:** 11 numeric + 9 categorical variables
* **Target:** `kwh/day`
* **Evaluation Metrics:**

  * **RMSE:** 7.05
  * **R² Score:** 0.27

Although the R² score is moderate, the model successfully captures baseline consumption patterns and can be improved further with feature selection and hyperparameter tuning.

---

## 🔍 Clustering Approach

* **Algorithm:** `KMeans`
* **Number of Clusters:** 4
* **Features Used:** Household size, demographics, income, education, and `kwh/day`
* **Result:** Segmented households into low, moderate, high, and extreme energy consumers
* **Visualization:** Scatter plot showing clusters based on `income` vs. `kwh/day`

---

## 📊 Power BI Dashboard

The dashboard provides a **visual, interactive way to explore the dataset** and insights:

### **1️⃣ Communicating the Problem & Insights**

* **Summary Cards:** Total households, average energy consumption, min/max usage
* **Problem Statement:** High variance in energy consumption leading to inefficiencies
* **Goal:** Identify patterns to recommend energy-saving strategies

### **2️⃣ Interactivity**

* **Slicers:**

  * Dwelling type
  * Heating source
  * Energy class
  * Awareness level
* **Filters:** Date range, household size
* **Drill-down:** From area-level energy usage to individual households

### **3️⃣ Charts Used**

* **Pie/Donut Chart:** Distribution of households by `energy_class`, recycling adoption, or awareness level
* **Bar/Column Chart:** Average energy consumption by dwelling type or heating source
* **Line/Area Chart:** Energy consumption trend over time
* **Map Visualization:** Energy consumption by `area_code`
* **Cluster Plot:** Household segments from KMeans

### **4️⃣ Innovative Features**

* **Predicted vs. Actual Consumption:** Displays results from the regression model
* **Custom Tooltip:** Shows detailed household information on hover
* **What-If Analysis:** Interactive parameter sliders to simulate changes in energy efficiency

---

## 🚀 Innovation

* **Ensemble Learning:** Enhanced predictions by combining multiple decision trees
* **Dynamic Clustering:** Allows changing the number of clusters to explore different segmentation levels
* **Scenario Simulation:** Power BI "What-If" parameters for projecting the impact of adding smart devices or improving energy class

---

## 📈 Evaluation

* **Regression:**

  * RMSE = `7.05`
  * R² = `0.27`
* **Clustering:**

  * Silhouette Score (can be computed for validation)
* **Dashboard Performance:** User-tested interactivity with filters and slicers

---

## 🛠️ Tools & Technologies

* **Python:** Data preprocessing, ML modeling
* **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn
* **Power BI:** Interactive dashboard and visualization
* **Dataset:** Household energy consumption CSV

---

## 📌 How to Use

1. Clone or download this repository
2. Open `cleaned_household_data.csv` in Power BI
3. Import visualizations as described
4. Use slicers and filters to explore household segments
5. (Optional) Run the Python scripts to retrain the model or adjust clustering

---

## ✅ Conclusion

This project demonstrates how data analytics and machine learning can be combined with powerful visualization tools like Power BI to gain actionable insights. The findings can help policymakers and energy providers:

* Identify high-consuming households
* Promote energy-efficient appliances
* Implement targeted awareness campaigns
* Monitor environmental sustainability initiatives