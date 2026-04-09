# Coffee Sales Data Analysis & Prediction

## Project Overview

This project analyzes coffee vending machine sales data to understand customer behavior, product demand, and sales trends over time. It also applies machine learning techniques to predict coffee sales based on various influencing factors.

The project includes data cleaning, exploratory data analysis (EDA), visualization, and predictive modeling to extract meaningful insights and support business decision-making.

---

## Objectives

- Analyze customer purchasing behavior  
- Identify top-selling coffee products  
- Understand sales trends across time (hour, day, month)  
- Explore payment method preferences  
- Build and evaluate machine learning models for sales prediction  
- Generate actionable business insights  

---

## Dataset

- Source: Coffee Vending Machine Dataset  
- Records: 1133 transactions  
- Features: Date, Time, Payment Type, Card, Coffee Type, Sales Amount  
- Target Variable: `money` (sales revenue)  

---

## Exploratory Data Analysis (EDA)

### Key insights:

- Milk-based coffees like **Latte, Cappuccino, and Americano with Milk** generate the highest revenue  
- Customers prefer **card/digital payments over cash**  
- Sales are higher during **morning and evening hours**  
- Weekly sales remain relatively consistent with slight variations  
- Different coffee types have **peak demand at different times of the day**  

EDA was supported with visualizations such as bar plots, line charts, histograms, and heatmaps.

---

## Machine Learning Approach

### Models Implemented

- Linear Regression (baseline model)  
- Random Forest Regressor (final model)  

### Key Techniques

- Data preprocessing and handling missing values  
- Feature engineering:
  - Extracted month, day, and hour from datetime  
  - Encoded categorical variables  
- Train-test split for model evaluation  

---

## Model Performance

- Linear Regression:
  - MSE ≈ 15.65  
  - R² ≈ 0.16 (low performance)  

- Random Forest Regressor:
  - MSE ≈ 0.57  
  - R² ≈ 0.97 (high accuracy)  

Random Forest significantly outperformed Linear Regression.

---

## Feature Importance

Key factors influencing coffee sales:

- **Payment Method (cash_type)** → Highest impact  
- **Coffee Type (coffee_name)** → Strong influence  
- **Time Features (hour, day)** → Moderate impact  
- **Month** → Minimal influence  

---

## Business Usage

This project can help businesses to:

- Optimize inventory based on popular coffee types  
- Improve payment systems for better customer experience  
- Plan staffing based on peak hours  
- Design targeted promotions for specific time periods  

---

## Limitations

- Small dataset (limited to 1133 records)  
- Does not include external factors (weather, location, promotions)  
- Predictions may not generalize to all coffee businesses  
- Real-time data not included  

---

## Tools & Technologies

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Repository Contents

- Coffee_sales.ipynb → Complete analysis and ML model  
- index.csv → Dataset used  
- README.md → Project documentation  

---

## Author

**Vikas Gowda V**  
Aspiring Data Analyst / Data Scientist  

---

## Conclusion

This project demonstrates a complete data analysis and machine learning workflow on coffee sales data. The analysis highlights key factors such as product type and payment method that significantly influence sales. Time-based trends provide additional insights into customer behavior.

The Random Forest model achieved high accuracy, making it suitable for predicting coffee sales. Overall, the project provides valuable insights that can help businesses optimize operations, improve customer experience, and maximize revenue.
