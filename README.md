# 🏡 Lasso, Ridge, and Polynomial Regression

This project explores **Regularization techniques (Ridge & Lasso)** and **Polynomial Regression** using a real-estate dataset.  
The goal is to compare models, analyze overfitting, and understand the impact of multicollinearity in regression.

---


### 🔹 Ridge Regression – Predicting House Prices


- **Dataset:** [House Prices Dataset](https://drive.google.com/file/d/1FDbOghfF0PbG7F8T1TNjK2U9c0BzDZTJ/view?usp=sharing)

- 
- **Features:**
- 
  - `size_m2` → Size of the house (in square meters)  
  - `bedrooms` → Number of bedrooms  
  - `bathrooms` → Number of bathrooms  
  - `distance_city` → Distance to city center (km)  
  - `age_years` → Age of the property (years)
 
  - 
- **Target:**  
  - `price_k` → House price (in thousands)

---

## 🎯 Scenario


A **real-estate agency** wants to predict house prices.  
However, **`size_m2` and `bedrooms` are highly correlated** → causing **multicollinearity** problems in OLS (Ordinary Least Squares).  

- We fit both:
- 
  - **OLS Regression**
  - **Ridge Regression**
  - 
- Then compare:
- 
  - **Coefficients** (stability & shrinkage)
  - **R² score** (model performance)

---

## 🔎 Why Ridge Regression?


- OLS suffers when features are highly correlated → coefficients become unstable & inflated.  
- **Ridge Regression** adds an **L2 penalty** → shrinks coefficients, reduces variance, and improves generalization.  
- In this scenario, Ridge handles the correlation between `size_m2` and `bedrooms` better, giving **more reliable predictions**.

---

## 📊 Results

- **OLS:** High variance, unstable coefficients due to multicollinearity.  
- **Ridge:** More stable coefficients, better R², improved generalization.  

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn (LinearRegression, Ridge)  


---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Thiyanesh07/Ridge-Lasso-Regression.git
```

```

## 📖 Learnings

- Effect of multicollinearity on regression models.

- How Ridge & Lasso regularization improve stability.

- Importance of Polynomial Regression in capturing non-linear relationships.

## ✨ Future Work

- Extend to Lasso Regression → feature selection by driving coefficients to zero.

- Apply Polynomial Regression for non-linear trends in housing data.

- Hyperparameter tuning with GridSearchCV.
