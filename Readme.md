# 🏡 Household Energy Consumption Analysis & Dashboard

## 📌 Introduction

The **Household Energy Consumption Analysis** project explores energy usage patterns across households to provide actionable insights for improving efficiency.
We combined **Python (Machine Learning)** and **Power BI** to:

* 🔮 Predict household energy consumption
* 🔑 Segment households using clustering
* 📊 Create an **interactive dashboard** for decision-making

---

## 🎯 Objectives

✔️ Clean and preprocess the dataset for accurate analysis
✔️ Engineer features for machine learning models
✔️ Build a **Random Forest regression model** for `kWh/day` prediction
✔️ Apply **KMeans clustering** to group households by consumption
✔️ Visualize insights through **Power BI dashboards**
✔️ Add innovative analytics features like **ensemble learning** and **what-if simulation**

---

## 📂 Dataset Overview

* **Total Records:** `188 households`
* **Features:** `38 columns`

### 🔑 Key Columns

* **🏠 House Characteristics:** `dwelling`, `dwelling_grade`, `household_m2`, `bedrooms`, `heating_source`
* **👨‍👩‍👧 Demographics:** `occupants`, `children`, `teenagers`, `adults`, `elders`
* **💰 Socioeconomic:** `income`, `education_index`, `recycling`, `awareness`
* **⚡ Energy Metrics:** `energy_class`, `thermostats`, `smart_plugs`, `water_heater`, `kwh/day`, `hdd`, `cdd`
* **⏳ Time Metrics:** `start`, `end`, `days`

---

## 🔧 Data Cleaning & Preprocessing

1. ✅ **Normalized column names** for uniformity
2. 🧹 Removed **duplicate headers** and **placeholder rows**
3. 🔄 **Handled missing values** (imputation or removal)
4. 💱 Converted **income** and other text-based numerics to integers
5. 🔢 **Encoded categorical variables** for modeling
6. ⚖️ Standardized numerical features using `StandardScaler`

---

## 🤖 Machine Learning Implementation

* **Algorithm:** `RandomForestRegressor`
* **Features:** 11 numeric + 9 categorical
* **Target Variable:** `kwh/day`

### 📊 Model Performance

* RMSE = **7.05**
* R² Score = **0.27**

> ⚠️ Although the R² score is moderate, the model establishes a strong baseline and can be improved further with feature selection and hyperparameter tuning.

---

## 🔍 Clustering Approach

* **Algorithm:** `KMeans`
* **Clusters:** `4` household segments
* **Input:** Household size, demographics, income, education, and `kwh/day`
* **Output:** Segmentation of low, medium, high, and extreme energy users
* **Visualization:** Scatter plot (`income` vs. `kwh/day`) with cluster coloring

---

## 📊 Power BI Dashboard

The dashboard transforms complex analysis into **actionable, interactive insights**:

### 1️⃣ Communicating the Problem & Insights

* **Summary Cards:** Total households, average usage, min/max consumption
* **Problem Statement:** Wide energy usage variance causing inefficiencies
* **Goal:** Identify patterns and recommend efficiency strategies

### 2️⃣ Interactivity

* **Slicers:** Dwelling type, heating source, energy class, awareness level
* **Filters:** Date range, household size
* **Drill-down:** Area-level to household-level usage

### 3️⃣ Charts

* 🥧 **Pie/Donut:** Energy class, recycling adoption, awareness level
* 📊 **Bar/Column:** Avg. usage by dwelling type or heating source
* 📈 **Line/Area:** Energy consumption trends
* 🗺️ **Map:** Area-wise consumption (`area_code`)
* 🔑 **Cluster Plot:** Visualizing KMeans household segmentation

### 4️⃣ Innovative Features

* 🔮 **Predicted vs. Actual Consumption** (from ML model)
* 🛠️ **Custom Tooltips** with detailed info
* 🤔 **What-If Analysis:** Simulate energy-saving actions (e.g., adding smart plugs)

---

## 🚀 Innovation

* **Ensemble Learning:** Boosting predictions with decision trees
* **Dynamic Clustering:** Adjustable number of segments for exploration
* **Scenario Simulation:** Power BI "What-If" analysis for energy efficiency planning

---

## 📈 Evaluation

* **Regression:** RMSE = `7.05`, R² = `0.27`
* **Clustering:** (Optional) Silhouette Score for validation
* **Dashboard:** Tested for interactivity and responsiveness

---

## 🛠️ Tools & Technologies

* 🐍 **Python:** Data preprocessing, ML modeling
* 📚 **Libraries:** Pandas, Scikit-learn, Matplotlib, Seaborn
* 📊 **Power BI:** Dashboard and visualization
* 💾 **Dataset:** `household_energy.csv`

---

## 📌 How to Use

1. Clone this repository
2. Open `cleaned_household_data.csv` in Power BI
3. Build visuals as described in the README
4. Use slicers and filters to explore segments
5. (Optional) Run Python scripts to retrain models or change clustering

---

## ✅ Conclusion

This project demonstrates the synergy between **Machine Learning** and **Power BI**, showing how data can drive energy efficiency policies.

**Benefits:**

* Identify high-consuming households
* Target appliance upgrades and smart device installations
* Design awareness campaigns for low-awareness groups
* Monitor sustainable energy initiatives effectively

---

## 📂 Repository Structure

```
📦 Household-Energy-Analysis
 ┣ 📜 README.md
 ┣ 📂 notebooks
 ┃ ┣ analysis1.ipynb
 ┃ ┣ analysis2.ipynb
 ┃ ┣ analysis3.ipynb
 ┃ ┗ analysis4.ipynb
 ┣ 📂 screenshots
 ┃ ┣ Img.png
 ┃ ┣ Img_1.png
 ┃ ┗ ...
 ┣ 📜 cleaned_household_data.csv
 ┗ 📜 requirements.txt
```

---

## 🖼️ Screenshots

Below are dashboard previews (more in `/screenshots`):

![Dashboard](screenshots/Img.png)
![Clustering](screenshots/Img_1.png)
