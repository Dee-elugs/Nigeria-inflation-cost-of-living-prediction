### **Project Overview**

This project analyzes Nigeria’s inflation trends and cost-of-living dynamics using historical economic data. It explores how changes in consumer price indices (CPI), food prices, and crude oil prices relate to headline inflation, and builds a machine learning model to predict short-term inflation trends.
The goal of the project is to demonstrate a complete data science workflow, from data cleaning and exploratory analysis to feature engineering and predictive modeling, using real Nigerian macroeconomic data.
-------

### **Dataset**

The dataset contains monthly Nigerian economic indicators, including:
Headline inflation rate
Consumer Price Index (CPI) components (Food, Energy, Transport, Health, etc.)
Crude oil prices, production, and exports
-------

### ** Key note:**

CPI values represent price index levels, not inflation rates. CPI-based inflation rates were calculated using month-on-month percentage changes.
-------

### **Tools & Technologies**

Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
Jupyter Notebook
-------

### **Exploratory Data Analysis**
**The analysis focuses on:**

Long-term trends in Nigeria’s headline inflation
Cost-of-living pressures across key CPI categories
The relationship between food prices, energy costs, and inflation volatility

**Key visualizations include:**

Headline inflation trends over time
CPI component trends for food, energy, and transport
Comparison of actual vs predicted inflation values
-------

### **Feature Engineering**
To prepare the data for modeling:
CPI index values were converted to monthly inflation rates using percentage change
Lag features were created to capture inflation persistence:
Previous month inflation
Previous month food inflation
Previous month crude oil price
Rows with missing values introduced by lagging were removed
-------

### **Modeling Approach**

A Random Forest Regressor was used to predict Nigeria’s headline inflation rate.
Train-test split respected time order (no shuffling)
Model performance was evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
Model Performance
MAE: ~4.9 percentage points
RMSE: ~7.2 percentage points
Given the volatility of inflation and structural economic shocks, this performance is considered reasonable for macroeconomic forecasting.
-------

### **Key Insights**

Inflation in Nigeria shows strong persistence, with previous months’ inflation playing a major role in predictions
Food-related price changes are a significant driver of headline inflation
Macroeconomic inflation is difficult to predict precisely due to policy shifts, supply shocks, and external factors
-------

### **Conclusion**
This project demonstrates how machine learning can be applied to real-world economic data to extract insights and generate short-term inflation forecasts. Rather than focusing on perfect accuracy, the emphasis is on correct methodology, economic reasoning, and clear interpretation of results.
