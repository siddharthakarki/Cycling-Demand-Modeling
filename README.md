# 🚴‍♂️ **Cycling Demand Modelling**

## 📌 Project Overview  
This project aims to develop a **regression model** to predict **bike rental demand** in a bike-sharing system based on various factors such as **temperature, humidity, weather conditions,** and **time of the day**. The dataset is analyzed to understand how **weather** and **temporal factors** influence **bike rentals** and to create a model for **demand forecasting**.

## 📊 Dataset Information  
- **Source**: [UCI Bike Sharing Dataset](https://archive.ics.uci.edu/dataset/275/bike+sharing+dataset)  
- **Variables**:  
  - **`cnt`**: Number of **bike rentals** on the corresponding day.  
  - **`mnth`**: Month of the year (1 to 12).  
  - **`weekday`**: Day of the week (0 = Sunday, 1 = Monday, ...).  
  - **`workingday`**: Dummy variable (1 = workday, 0 = weekend or holiday).  
  - **`weathersit`**: Weather conditions (1 = clear, 2 = misty, 3 = light snow/rain).  
  - **`temp`**: Temperature in Celsius (normalized between 0 and 1).  
  - **`atemp`**: "Feeling" temperature in Celsius (normalized between 0 and 1).  
  - **`hum`**: Humidity (normalized between 0 and 1).  
  - **`windspeed`**: Windspeed (standardized between 0 and 1).  

---

## 🚀 **Key Objectives**  

✔️ **Descriptive Analysis**: Understand the relationship between **bike rentals** and key factors like **temperature, weather**, and **time**.  
✔️ **Regression Model**: Build a **linear regression** model to predict **bike rentals**.  
✔️ **Feature Selection**: Identify the most significant predictors using **AIC** and **backward elimination**.  
✔️ **Model Evaluation**: Assess the model using **R²**, **AIC**, and **residual analysis**.  
✔️ **Non-linear Effects**: Explore the impact of **temperature** using **quadratic terms** to capture potential non-linear relationships.

---

## 🔍 **Methodology & Statistical Approach**  

### ✅ 1. Descriptive Analysis  
- Summarize **bike rental distributions** across different **weather conditions** and **months**.  
- Visualize data relationships using **scatter plots**, **box plots**, and **heatmaps**.  

### ✅ 2. Linear Regression Model  
- **Null Hypothesis (H₀)**: No significant relationship between bike rentals and weather or temporal factors.  
- **Alternative Hypothesis (H₁)**: At least one factor significantly influences bike rentals.  
- **Test Used**: **Multiple Linear Regression** with all available predictors.  
- **Key Focus**: Analyze **temperature's** non-linear impact using quadratic terms (e.g., `temp_sq`).  

### ✅ 3. Feature Selection  
- **Backward Elimination** with **AIC** to remove non-significant variables.  
- Use **VIF** to assess **multicollinearity** and refine the model.

### ✅ 4. Model Evaluation  
- **Assess R²**: Proportion of variance explained by the model.  
- **Residual Analysis**: Check for **linearity**, **heteroscedasticity**, and **normality** of residuals.  
- **AIC**: Track the goodness of fit while penalizing for more variables.  

---

## 📈 **Key Findings**  

### 📍 Descriptive Insights  
✔️ **Temperature** showed a strong **positive correlation** with bike rentals (r = 0.63).  
✔️ **Age groups** had varying levels of **bike rental demand**, with **cooler months** (October, November) showing higher usage.  

### 📍 Regression Model Results  
✔️ The **final model** explained **60.6%** of the variance in bike rentals (R² = 0.606).  
✔️ **Key predictors**: **Temperature** (linear and quadratic), **workingday**, **windspeed**, and **humidity**.  
✔️ **Polynomial term for temperature**: The quadratic term for temperature significantly improved the model.  

### 📍 Residual Analysis  
✔️ **Heteroscedasticity** was observed, suggesting that **model fit** varied across the rental levels.  
✔️ Residual plots showed **non-constant variance**; future iterations could explore **weighted least squares regression**.  

---

## 🛠 **Technologies Used**  

📊 **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `statsmodels`  
📝 **Jupyter Notebook** for interactive analysis  
🔧 **Markdown** for documentation and **LaTeX** for mathematical formulations  

---

## 📢 **Conclusion & Future Work**  

- 🔹 **Weather and temporal factors** significantly influence **bike rental demand**.  
- 🔹 **Temperature** (especially its quadratic term) plays a **crucial role** in predicting demand.  
- 🔹 The **model can be refined** by exploring **heteroscedasticity** and **multicollinearity** further.  
- 🔹 Future work could include incorporating **local events**, **holidays**, and **demographic trends** for more precise predictions.  

---

## 💡 **Contributors**  

👤 **Siddhartha Karki**  
📧 Sidkarki999@gmail.com  
🌐 https://www.linkedin.com/in/siddhartha-karki 

📌 **Support & Contributions**  
⭐ **If you found this project useful, give it a star!**  
💬 **Feedback and contributions are welcome!** 🎯
