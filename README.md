# **Time Series Forecasting: Stock Prices & Temperature Trends** 📈🌡️  

## **Overview**  
This project applies **time series forecasting techniques** to two datasets:  
- **Non-Seasonal Data**: **Dabur Stock Prices** (Yahoo Finance)  
- **Seasonal Data**: **Chennai Temperature Trends**  

It leverages **ARIMA, SARIMA, and GARCH models** to analyze and predict financial and climate data trends.

---

## **Project Structure**  

📂 **Non Seasonal_E Navaneet Kumar.ipynb** - Time series analysis & forecasting of stock prices.  
📂 **Seasonal_E Navaneet Kumar.ipynb** - Time series analysis & forecasting of seasonal temperature trends.  
📂 **data/** - Folder containing datasets.  
📂 **README.md** - Project documentation.  

---

## **Key Features**  

✅ **Data Preprocessing**: Handling missing values, outliers, and converting time series to stationary data.  
✅ **Stationarity Tests**: **ADF Test** for stationarity verification.  
✅ **Forecasting Models**:  
   - **ARIMA**: Forecasts non-seasonal stock prices.  
   - **GARCH**: Models volatility clustering in stock price returns.  
   - **SARIMA**: Captures seasonal variations in temperature data.  
✅ **Residual Analysis**: **Ljung-Box, PACF, ACF tests** for model validation.  
✅ **Visualization**: Time series plots, ACF/PACF, residual diagnostics, and forecasting visualizations.  

---

## **Datasets**  

📌 **Dabur Stock Prices (2012-2022)** - **Yahoo Finance**  
📌 **Chennai Temperature Data** - Historical monthly temperatures  

---

## **Project Workflow**  

### **1️⃣ Data Preprocessing**  
✔️ Convert date columns to datetime format.  
✔️ Handle missing values & remove anomalies.  
✔️ Apply **log transformations & differencing** to ensure stationarity.  

### **2️⃣ Stationarity & Model Selection**  
✔️ **ADF Test** - Check if time series is stationary.  
✔️ **ACF & PACF Plots** - Identify AR and MA terms.  
✔️ **Ljung-Box Test** - Ensure residuals are not autocorrelated.  

### **3️⃣ Forecasting Models**  

#### **Non-Seasonal Stock Price Data (Dabur)**  
📈 **ARIMA(p,d,q)** – Best model based on **AIC/BIC criteria**.  
📈 **GARCH(p,q)** – Captures **volatility clustering** in stock returns.  

#### **Seasonal Temperature Data (Chennai)**  
🌡️ **SARIMA(p,d,q)(P,D,Q,s)** – Captures seasonal variations.  

### **4️⃣ Model Evaluation & Interpretation**  
✔️ Analyze **residuals for normality & independence**.  
✔️ **Compare models** based on forecast accuracy.  
✔️ **Visualize predictions** with confidence intervals.  

---

## **Results & Insights**  

📌 **Stock Market Predictions**  
✅ **Best ARIMA Model**: **ARIMA(7,0,9)** based on AIC score.  
✅ **Best GARCH Model**: **GARCH(3,2)** effectively models stock volatility.  
✅ **Stock Returns Analysis**: Significant **volatility clustering observed**.  

📌 **Temperature Forecasting**  
✅ **Best SARIMA Model**: **SARIMA(2,1,2)(1,1,1,12)** for seasonal temperature fluctuations.  
✅ **Temperature Trends**: Yearly seasonality with **periodic peaks** detected.  

---

## **Technologies Used**  

🟢 **Python**  
🟢 **Libraries**: Pandas, NumPy, Matplotlib, Seaborn  
🟢 **Time Series Modeling**: Statsmodels, ARCH, Scipy  
🟢 **Forecasting**: ARIMA, SARIMA, GARCH  

---

## **Future Enhancements 🚀**  

✅ **Implement LSTMs & Deep Learning** for time series forecasting.  
✅ **Hybrid ARIMA-GARCH Models** for enhanced stock prediction.  
✅ **Deploy Real-time Forecasting Dashboard** using **Power BI / Tableau**.  

---

## **License**  

📜 This project is licensed under the **MIT License**.  
