# 🏠 House Price Prediction

![Python](https://img.shields.io/badge/Python-3.8%2B-blue) 
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)

A complete **machine learning workflow** to predict house prices using **linear regression, ridge regression, and polynomial features**.  
Built as part of learning **regression modeling for data science and analytics**.

---

## 📝 Description
This project analyzes a **real housing dataset (King County, USA)** to predict house prices.  
It includes **data cleaning, exploratory data analysis (EDA), and multiple regression models** to evaluate performance.

---

## ✨ Benefits
- Practice **end-to-end ML workflows** with `scikit-learn`.  
- Strengthens understanding of **EDA, regression, and evaluation metrics**.  
- Real-world dataset → practical data cleaning and imputation.  
- Builds portfolio credibility for **data science & analytics roles**.  

---

## 🔑 Features
- 📥 Load dataset (local or URL with NaN handling)  
- 🧹 Clean data (drop IDs, impute missing values)  
- 📊 Exploratory Data Analysis:  
  - Boxplot: Price vs Waterfront  
  - Regression plot: Price vs Sqft Above  
  - Top correlations with price  
- 🤖 Models:  
  - Baseline Linear Regression (single feature)  
  - Multi-feature Linear Regression  
  - Polynomial (deg=2) + Ridge with Train/Test split  
- ✅ Final comparison summary  

---

## 📂 File Structure
```
house-price-prediction-python/
│
├── King County House Price Prediction/
│   ├── main.py # Main program (data loading, EDA, modeling)
│   └── kc_house_data_NaN.csv # Dataset (with NaN values to be cleaned)
├── README.md # Project documentation
```

---

## ⚙️ How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/House_Price_Prediction.git
   cd House_Price_Prediction
   ```

2. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```

3. Run the program:
   ```bash
   python house_price_prediction.py
   ```

---

## 📊 Example Output
<details>
<summary>Click to view sample output</summary>

```bash
==============================
     DATA LOADED
==============================
Rows x Cols               : 21,613 x 21
Source                    : Local CSV

[ EDA • Top correlations with price ]
feature             corr_with_price
sqft_living         0.70
grade               0.67
sqft_above          0.60

[ MODEL SUMMARY ]
Baseline LinearRegression (sqft_living)   R²: 0.49
Multi-feature LinearRegression (11 feats) R²: 0.65
Poly (deg=2) + Ridge (α=0.1) — Test R²   : 0.81

Done ✔
```
</details>

---

## 👤 Author
**Abinash Prasana**  
📧 abinashprasana400@gmail.com  

---
