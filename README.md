# 🚗 Car Price Prediction Project

An end-to-end Machine Learning project designed to predict the resale value of used cars based on various features such as vehicle age, brand, driven kilometers, fuel type, and transmission.

## 📊 Project Overview
Predicting used car prices is a classic regression problem. This project walks through the entire data science workflow, including data cleaning, extensive feature engineering, exploratory data analysis (EDA), and model deployment tracking.

### 🛠️ Tech Stack & Libraries Used
* **Language:** Python
* **Environment:** Jupyter Notebook / VS Code
* **Data Manipulation:** `pandas`, `numpy`
* **Machine Learning:** `scikit-learn`
* **Model Serialization:** `pickle` (for exporting the trained model)

---

## 💡 Key Features Implemented

1. **Feature Engineering:**
   * Calculated precise vehicle age using the formula: 
     $$\text{Car\_Age} = 2026 - \text{Year}$$
   * Extracted clean, normalized automobile brand names directly from messy text fields using text-splitting and lowercasing techniques:
```python
     df['Brand'] = df['Car_Name'].str.split().str[0].str.lower()
     ```

2. **Exploratory Data Analysis (EDA):**
   * Investigated the statistical breakdown of the dataset using `.head()`, `.shape`, and target value distributions.
   * Analyzed how vehicle age and specific brands heavily influence final market pricing.

3. **Model Production:**
   * Exported the fully optimized pipeline to a serialized file (`Car Price Prediction.pkl`) for clean integration into potential web applications.

---

## 📂 Repository File Structure

* `Car Price Prediction.ipynb` — The primary Jupyter Notebook containing all data cleaning, EDA, and regression modeling.
* `car_data.csv` — The raw features dataset utilized for training and evaluation.
