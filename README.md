# 🚗 Car Price Prediction using Machine Learning

This project aims to **predict the selling price of used cars** based on various features such as age, mileage, fuel type, transmission, and more.  
The goal is to compare multiple regression models and determine which performs best in predicting car prices.

---

## 📊 Project Overview

Predicting used car prices helps both buyers and sellers make data-driven decisions.  
In this project, we:

- Collected and preprocessed the dataset.  
- Engineered new insightful features.  
- Trained three machine learning models:  
  - **Linear Regression**  
  - **Decision Tree Regressor**  
  - **Random Forest Regressor**  
- Compared their performance using standard metrics.  
- Visualized the actual vs predicted prices for better understanding.

---

## 🧠 Models Used

| Model | Description |
|--------|--------------|
| **Linear Regression** | A simple baseline model assuming linear relationships between features and target. |
| **Decision Tree Regressor** | Non-linear model that splits data into regions for prediction. |
| **Random Forest Regressor** | Ensemble of decision trees; reduces overfitting and improves accuracy. |

---

## ⚙️ Features Used in Training

| Feature | Description |
|----------|-------------|
| `Present_Price` | Current ex-showroom price of the car |
| `Kms_Driven` | Total distance driven (in km) |
| `Car_Age` | Age of the car (in years) |
| `Kms_Per_Year` | Average distance driven per year |
| `High_Mileage` | Indicates if the car is high-mileage |
| `Price_Ratio` | Ratio of selling to present price |
| `Fuel_Type_Diesel`, `Fuel_Type_Petrol` | Encoded fuel type |
| `Seller_Type_Individual` | Encoded seller type |
| `Transmission_Manual` | Encoded transmission type |
| `Age_Category_Mid`, `Age_Category_Old`, `Age_Category_Very Old` | Age group categories |

**Total Features:** 13

---

## 📈 Results Summary

| Metric | Linear Regression | Decision Tree | Random Forest |
|---------|-------------------|----------------|----------------|
| R² Score(Higher=Better) | 0.889 | 0.956 | 0.951 |
| RMSE(Lower=Better) | 1.197 | 0.758 | 0.793 |
| MAE(Lower=Better) | 0.892 | 0.480 | 0.450 |


✅ **Verdict:** Random Forest gives the most accurate and stable predictions, making it the best choice for this dataset.

---

## 🎨 Visualizations

### 1. Actual vs Predicted Prices
A scatter plot comparing actual and predicted selling prices for all three models.

*(Saved as `predicted_vs_actual_comparison.png`)*

### 2. Model Performance Comparison
Bar charts and evaluation metrics used to visualize the error comparison across models.

*(Saved as `Model_Performance_Comparison.png`)*

### 3. Feature Importance
Tells us that on what Features does our Random Forest model relies the most to predict correct answers

*(Saved as `Feature_Importance.png`)*

---

## 🧩 Technologies Used

- **Python 3.10**
- **Pandas** – Data manipulation  
- **NumPy** – Numerical computations  
- **Matplotlib / Seaborn** – Data visualization  
- **Scikit-learn** – Model building and evaluation  

---

## 🚀 How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/Saqib-develops/Car_price_prediction.git
   cd Car-price-prediction

2. Install Dependencies:
    ```bash
   pip install -r requirements.txt

3. Run the Notebook:
   ```bash
   jupyter notebook used_cars.ipynb

