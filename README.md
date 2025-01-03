# Finance-Forecasting
### Project Overview: Financial Time Series Analysis and Forecasting

This project, developed by **Framba Matteo, Ph.D. in Mathematics**, on **December 31, 2024**, focuses on analyzing financial time series data and implementing predictive models. It combines advanced statistical methods with machine learning techniques to explore relationships between financial assets and forecast their future behavior. 

The work is organized into two primary parts: 

---

## **Part I: Forecast with Correlation**

### **Objective**:
This section aims to identify and quantify relationships between financial assets using correlation analysis and Granger causality tests. It then builds predictive models to forecast daily returns.

### **Highlights**:
1. **Data Collection**:
   - Retrieves daily closing prices for commodities, indices, currencies, and bonds from January 2020 to December 2023 using the `yfinance` library.
   - Combines financial assets into a unified dataset for analysis.

2. **Exploratory Data Analysis**:
   - Visualizes trends and patterns in the financial series.
   - Computes a correlation matrix to identify linear dependencies.

3. **Granger Causality Testing**:
   - Determines whether one time series can predict another based on lagged information.
   - Results are visualized using a heatmap of p-values and an influence summary.

4. **Predictive Modeling**:
   - Implements **Random Forest Regressors** to forecast daily returns based on identified influencers.
   - Evaluates models using Mean Squared Error (MSE) and accuracy in predicting return signs.
   - Provides visualizations of predicted vs. actual returns and highlights model performance with bar charts.

---

## **Part II: Forecast with Stochastic Processes**

### **Objective**:
This section uses advanced stochastic modeling techniques, including **GARCH models** and **Monte Carlo simulations**, to forecast the future prices of financial assets, focusing on Crude Oil.

### **Highlights**:
1. **Volatility Modeling with GARCH(1,1)**:
   - Models log returns of Crude Oil prices to capture volatility dynamics.
   - Forecasts future volatility over a 30-day horizon.

2. **Monte Carlo Simulations**:
   - Simulates 180-day future price paths for Crude Oil based on GARCH-derived volatility.
   - Computes the median prediction, 25th percentile, and 75th percentile to quantify uncertainty.

3. **Visualization**:
   - Plots historical data alongside simulated price paths.
   - Compares predicted prices with actual data to evaluate accuracy using Mean Squared Error (MSE).

---

### **Key Findings and Implications**:
- **Correlation and Predictive Modeling**:
   - Strong interdependence is observed among certain financial assets (e.g., Crude Oil and Brent Crude).
   - Random Forest models show high accuracy for certain assets but struggle with others (e.g., Natural Gas and EUR/USD).

- **Stochastic Forecasting**:
   - GARCH-based volatility modeling captures short-term dynamics effectively.
   - Monte Carlo simulations provide a robust framework for quantifying uncertainty in price predictions, but large market fluctuations remain challenging to predict.

---

### **Who Is This For?**
This project is suitable for:
- Financial analysts exploring time series forecasting techniques.
- Researchers studying Granger causality and stochastic models.
- Data scientists interested in machine learning applications in finance.

### **How to Use the Project**:
The project is divided into clearly structured code blocks, with explanations for each step. Users can replicate the analysis or adapt it for their datasets and objectives. 



