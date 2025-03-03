# 📊 Comparison of Domestic Tourist Predictions in Denpasar Using Holt-Winters and SARIMA Methods  

## 👥 Author  
**Jihan Fadila**  
📧 Email: jihan4han97@gmail.com

## 📌 Introduction  
Denpasar, the capital of Bali, plays a crucial role in Indonesia's tourism industry. **Fluctuations in tourist numbers** can significantly impact the local economy, making accurate **visitor predictions essential** for effective planning.  

This study **compares two time-series forecasting methods**:  
- **Holt-Winters Exponential Smoothing**  
- **Seasonal Autoregressive Integrated Moving Average (SARIMA)**  

By analyzing historical tourist arrival data, we aim to determine the **most accurate model** for predicting domestic tourist visits to Denpasar.  

---

## 🎯 Research Objectives  
1. **Compare the accuracy** of Holt-Winters and SARIMA in forecasting domestic tourist arrivals.  
2. **Identify the best method** for supporting tourism planning and decision-making.  
3. **Provide recommendations** for optimizing marketing strategies and resource allocation.  

---

## 🛠 Methodology  
### **1. Data Collection**  
- Data was sourced from **Badan Pusat Statistik (BPS) Indonesia** and the **Denpasar Tourism Office**.  
- The dataset includes **historical domestic tourist arrival records**.  

### **2. Forecasting Models**  
#### **Holt-Winters Exponential Smoothing**  
- A **time-series forecasting method** that incorporates **trend and seasonal components**.  
- The additive model was selected due to its **consistent seasonal fluctuations**.  

**Holt-Winters Equations:**  
- **Level Update:**  
  **Lt=α(Yt​−St−m​)+(1−α)(Lt−1​+Tt−1​)**
- **Trend Update:**  
  **Tt=β(Lt​−Lt−1​)+(1−β)Tt−1**
- **Seasonal Component:**  
  **St=γ(Yt​−Lt​)+(1−γ)St−m​**
  
where **α, β, γ** are smoothing parameters and **m** is the seasonal period.  

#### **SARIMA (Seasonal ARIMA)**  
- A **statistical model** that accounts for **seasonality and autocorrelation** in time-series data.
- SARIMA model is defined as **SARIMA(p, d, q) × (P, D, Q)m**, where:  
  - **p, d, q** = ARIMA parameters  
  - **P, D, Q** = Seasonal components  
  - **m** = Seasonal period  

---

## 📊 Results & Discussion  
### **Model Performance Comparison**  
To evaluate model accuracy, we used the **Mean Absolute Percentage Error (MAPE)** metric:

| Model  | MAPE (%) |
|--------|---------|
| **Holt-Winters** | **3.25** |
| **SARIMA** | 12.85 |

**Findings:**  
✅ Holt-Winters **outperformed SARIMA**, providing more accurate predictions.  
✅ SARIMA exhibited **higher errors** due to **larger deviations from actual data**.  
✅ The **seasonality and trend smoothing** of Holt-Winters made it a **better choice for tourism forecasting**.  

### **Visualization of Predictions**  
- **Holt-Winters Prediction (Orange Line) vs. Actual Data (Blue Line):**  
  - The model closely follows seasonal patterns with minimal deviations.  
- **SARIMA Prediction (Red Line) vs. Actual Data (Blue Line):**  
  - The model captures general trends but has **higher variance** in seasonal peaks.  

---

## 🏆 Conclusion  
- The **Holt-Winters method is the best choice** for predicting domestic tourist arrivals in Denpasar.  
- The model’s **low error rate (3.25%)** makes it **reliable for tourism planning**.  
- **SARIMA**, while effective for certain datasets, was **less accurate in this case** due to **higher prediction variance**.  

### **Impact & Future Work**  
🔹 **Accurate forecasting** helps stakeholders **optimize marketing strategies and resource management**.  
🔹 Future research can explore **hybrid models (e.g., Holt-Winters + Machine Learning)** to improve accuracy.  
🔹 Implementing **real-time prediction dashboards** using Python and MLflow can **enhance decision-making**.  
