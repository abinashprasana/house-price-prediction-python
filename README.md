# 🏡 King County House Price Prediction

This project predicts **house prices** in King County using **machine learning** techniques.  
It combines **data cleaning**, **exploratory data analysis (EDA)**, and **regression models** to understand how different features (like square footage, bedrooms, bathrooms, etc.) influence property prices.

---

## 📝 Description
The project loads and cleans the **King County house dataset** (with NaN values), explores correlations, visualizes relationships, and trains multiple regression models.  
It demonstrates a complete **data science workflow**:  
from raw dataset → cleaning → analysis → modeling → evaluation.

---

## ✨ Benefits
- Helps understand how **location & features** affect house prices  
- Demonstrates a **real-world ML pipeline** from data prep to model evaluation  
- Useful practice for **data science, AI, and analytics roles**  
- Beginner-friendly but extendable to more advanced models

---

## 🔑 Features
- 📂 Loads dataset (local CSV or online link)  
- 🧹 Cleans data: removes IDs, imputes missing values  
- 📊 Exploratory Data Analysis (EDA) with Seaborn/Matplotlib  
- 📈 Correlation check of top features with price  
- 🤖 Multiple regression models:
  - Baseline Linear Regression (1 feature)  
  - Multi-feature Linear Regression  
  - Polynomial Regression + Ridge (train/test split)  
- ✅ Model evaluation with R² scores (train & test)

---

## 📂 File Structure
```
house-price-prediction-python/
├── main.py                  # Main program (data loading, cleaning, EDA, modeling)
├── kc_house_data_NaN.csv    # Dataset with house features and prices
└── README.md                # Project documentation
```

---

## ⚙️ How to Run
**Requirements:** Python 3.8+ and the following libraries:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

**Steps:**
1. Clone this repository  
   ```bash
   git clone https://github.com/<your-username>/house-price-prediction-python.git
   cd house-price-prediction-python
   ```
2. Place the dataset (`kc_house_data_NaN.csv`) in the project folder (or let the script fetch from URL).  
3. Run the main script:  
   ```bash
   python main.py
   ```
4. The program will:
   - Clean the dataset  
   - Show plots for EDA  
   - Train baseline & advanced models  
   - Print performance summary

---

## 📊 Example Output
```
======================================================================
                          DATA LOADED
======================================================================
Rows x Cols             : 21,613 x 21
Source                  : Local CSV

======================================================================
                       CLEANING SUMMARY
======================================================================
Missing values (before → after)
  bedrooms : 13 → 0
  bathrooms: 10 → 0

[ EDA • Top 10 correlations with price ]
      feature          corr_with_price
0     price               1.000000
1     sqft_living         0.702035
2     grade               0.667434
...

[ Model • Multi-feature Linear Regression ]
n_features : 11
R²         : 0.6531
Top 5 |coef| features:
   feature        abs_coef
0  sqft_living    321.44
1  grade          213.98
...

[ FINAL SUMMARY ]
Baseline LinearRegression (sqft_living)   R²: 0.4921
Multi-feature LinearRegression (11 feats) R²: 0.6531
Poly (deg=2) + Ridge (α=0.1) — Train R²  : 0.8547
Poly (deg=2) + Ridge (α=0.1) — Test  R²  : 0.8123

Done ✔
```

---

## 🚀 Possible Extensions
- Add **Random Forest / XGBoost** for better prediction  
- Deploy as a **Flask/Django web app** with user input form  
- Integrate **interactive dashboards** (Plotly/Dash)  

---

## 👤 Author
**Author: Abinash Prasana**
