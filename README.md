# 💎 Diamond Price Prediction – Machine Learning Application

A data-driven machine learning application built to accurately predict diamond prices using key attributes such as carat, cut, color, clarity, and dimensions.  
The project follows a **modular MVC architecture** and leverages **Scikit-learn** for model training, preprocessing, and evaluation.

---

## 🎯 Objective

To predict the price of a diamond based on its physical and qualitative attributes using advanced regression models, while ensuring high accuracy and interpretability.

---

## 🧠 Key Features

- 🧩 **MVC Architecture:** Structured project design separating data processing, model training, and visualization modules.  
- 📊 **Exploratory Data Analysis (EDA):** Detailed analysis of price distribution, feature correlations, and categorical trends.  
- ⚙️ **Data Preprocessing:** Handling missing values, encoding categorical features (cut, color, clarity), and feature scaling.  
- 🤖 **Model Training:** Implemented multiple regression models to compare performance and generalization.  
- 📈 **Model Evaluation:** Used metrics like R², RMSE, and MAE to measure predictive accuracy.  
- 💡 **Insights:** Identified **carat** as the most influential feature, followed by **cut** and **clarity**.

---

## 🛠️ Tech Stack

| Component | Technology |
|------------|-------------|
| **Language** | Python |
| **Libraries** | NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn |
| **Architecture** | MVC (Model-View-Controller) |
| **IDE/Tools** | Jupyter Notebook, VS Code |

---

## 🧩 Dataset Information

- **Total Records:** 193,000+ diamonds  
- **Features:**
  - `carat` – Weight of the diamond  
  - `cut` – Quality of the cut (Fair, Good, Very Good, Premium, Ideal)  
  - `color` – Diamond color grade (D–J, where D is best)  
  - `clarity` – Level of inclusions (I1 to IF)  
  - `x`, `y`, `z` – Dimensions in millimeters  
  - `depth`, `table` – Proportional measurements affecting light reflection  
  - `price` – Target variable (in USD)

---

## ⚙️ Implementation Steps

1. **Data Cleaning & Preprocessing**
   - Removed null or invalid entries.
   - Encoded categorical variables using LabelEncoder and OneHotEncoder.
   - Scaled numerical attributes using StandardScaler.

2. **Exploratory Data Analysis (EDA)**
   - Visualized relationships between features and price.
   - Detected outliers and assessed their impact.
   - Identified carat as the most correlated feature.

3. **Model Training**
   - Trained multiple regression models:
     - Lasso Regression  
     - Ridge Regression  
     - Decision Tree Regressor  
     - Random Forest Regressor  
     - Gradient Boosting Regressor

4. **Model Evaluation**
   - Used R², RMSE, and MAE as evaluation metrics.
   - Tuned hyperparameters using GridSearchCV.

---

## 📊 Model Performance

| Model | R² Score | RMSE (USD) | MAE (USD) |
|--------|-----------|-------------|------------|
| **Lasso** | 93.68% | 1013.87 | 675.07 |
| **Ridge** | 93.69% | 1013.90 | 674.05 |
| **Decision Tree** | 95.74% | 825.31 | 421.65 |
| **Random Forest** | **97.71%** | **610.78** | **311.80** |
| **Gradient Boosting** | 97.66% | 617.47 | 331.90 |

✅ **Best Model:** Random Forest Regressor (R² = 97.7%, RMSE ≈ \$610)

---

## 📈 Insights

- **Carat** has the strongest influence on price.  
- **Cut** and **Clarity** significantly affect pricing in mid-range diamonds.  
- Models with ensemble techniques (Random Forest, Gradient Boosting) outperformed linear models.  
- Achieved **R² = 97.7%**, demonstrating high predictive accuracy.

---

## 🚀 Getting Started

### 🔧 Prerequisites
Ensure you have the following installed:
- Python 3.8 or later  
- Jupyter Notebook (optional)  
- pip

### 📦 Installation
```bash
git clone https://github.com/Adarsh-Mishra15/diamond-price-prediction.git
cd diamond-price-prediction
pip install -r requirements.txt
