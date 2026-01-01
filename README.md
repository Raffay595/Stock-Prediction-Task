# Task 2: Predict Future Stock Prices (Short-Term)

## Objective
The objective of this task is to predict the **next day’s closing stock price** using historical stock market data.  
Regression-based machine learning techniques are applied to analyze short-term price movements.

---

## Dataset
- **Source:** Yahoo Finance  
- **Access Method:** `yfinance` Python library  
- **Stock Used:** Apple Inc. (AAPL)  
- **Time Period:** January 2023 – January 2025  

### Features Used:
- Open price  
- High price  
- Low price  
- Volume  

### Target Variable:
- Next day’s **Close price**

---

## Tools
- Python
- Jupyter Notebook
- yfinance
- pandas
- matplotlib
- scikit-learn

---

## Model Applied
- **Linear Regression**

The model is trained to predict the next trading day’s closing price using current day market features.  
Time-series order is preserved during training by disabling data shuffling.

---

## Workflow
1. Fetch historical stock data using Yahoo Finance API  
2. Preprocess and select relevant features  
3. Shift closing prices to create next-day prediction target  
4. Split data into training and testing sets  
5. Train regression model  
6. Evaluate model using Mean Squared Error (MSE)  
7. Visualize actual vs predicted closing prices  

---

## Results
- The model produces reasonable short-term predictions.
- Visualization shows that predicted prices closely follow actual trends.
- Due to market volatility, the model is **not suitable for long-term forecasting**.

---

## Key Learnings
- Handling time-series data correctly is critical for stock prediction tasks.
- Regression models can capture short-term trends but struggle with market uncertainty.
- Feature selection and proper preprocessing significantly impact model performance.

---
