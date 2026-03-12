# ✈️ Airline Flight Delay Prediction
### Predictive Analytics using Power BI, JMP, and Python

This project develops a **predictive analytics pipeline** to identify flights at risk of delay using operational airline data. The goal is to predict whether a flight will experience an **arrival delay of 15 minutes or more** using information available **before or shortly after departure**.

The analysis combines **exploratory analytics, statistical modelling, and machine learning** using tools including **Power BI, JMP, and Python**.

---

# 📊 Project Overview

Airline delays create cascading disruptions across airline networks, affecting:

- Passenger satisfaction
- Aircraft utilization
- Crew scheduling
- Operational efficiency
- Airline costs

Using historical flight data from the **U.S. Bureau of Transportation Statistics (BTS)**, this project analyzes operational patterns and develops machine learning models to predict delay risk.

---

# 🎯 Objective

Predict whether a flight will experience a **15+ minute arrival delay**.

Target Variable:
ARR_DEL15 = 1 → Flight delayed ≥ 15 minutes
ARR_DEL15 = 0 → Flight not delayed


The prediction uses **pre-departure operational features**, ensuring the model can be applied in real-world airline operations.

---

# 🛠 Tools & Technologies

| Tool | Purpose |
|-----|------|
| **Power BI** | Exploratory data analysis and visual insights |
| **JMP** | Statistical modelling and logistic regression |
| **Python** | Machine learning implementation |
| **Scikit-Learn** | Model development |
| **XGBoost** | Gradient boosting model |
| **LightGBM** | High-performance gradient boosting |
| **GitHub** | Version control and project documentation |

---

# 📁 Dataset

**Source:**  
U.S. Bureau of Transportation Statistics (BTS)

**Dataset:**  
Airline On-Time Performance Dataset

**Data Scope**

- ~30,000 flight records  
- ~65 variables  
- Flight-level operational details

The dataset includes information such as:

- Flight schedules
- Departure and arrival times
- Airline carriers
- Airport locations
- Taxi-out times
- Flight distance

---

# 🔎 Exploratory Data Analysis (Power BI)

Power BI dashboards were used to identify key operational patterns contributing to delays.

Key insights include:

- **Taxi-out congestion is a major contributor to delays**
- **Short-distance flights experience more frequent delays**
- **Certain airline carriers show higher delay probabilities**
- **Airport congestion significantly impacts delay propagation**

These insights guided feature selection for predictive modelling.

---

# ⚙️ Data Preprocessing

The dataset required extensive cleaning before modelling.

### Key preprocessing steps

- Removal of **identifier variables**
- Elimination of **data leakage variables**
- Feature engineering
- Missing value handling
- Class imbalance handling

### Feature Engineering Example

Distance values were grouped into operational categories:

| Distance | Category |
|------|------|
| 0 – 500 miles | Very Short |
| 500 – 1000 miles | Short |
| 1000 – 1500 miles | Medium |
| 1500 – 2500 miles | Long |
| 2500+ miles | Very Long |

This helped capture **non-linear delay patterns across routes**.

---

# 🤖 Machine Learning Models

The following models were implemented and compared.

| Model | Description |
|------|------|
| Logistic Regression | Interpretable baseline model |
| Random Forest | Tree-based ensemble |
| XGBoost | Gradient boosting model |
| Neural Network | Deep learning classifier |
| LightGBM | Optimized gradient boosting |

---

# 🏆 Model Performance Comparison

| Model | Accuracy | Delay Precision | Delay Recall | ROC AUC |
|------|------|------|------|------|
| Logistic Regression | 0.84 | 0.95 | 0.72 | 0.892 |
| Random Forest | 0.80 | 0.90 | 0.68 | 0.872 |
| XGBoost | 0.83 | 0.93 | 0.72 | 0.907 |
| Neural Network | 0.85 | 0.87 | 0.82 | 0.914 |
| **LightGBM (Best)** | **0.87** | **0.95** | **0.79** | **0.927** |

LightGBM delivered the **best overall predictive performance**.

---

# 🔍 Key Insights

Major operational drivers of airline delays include:

- **Taxi-out time**
- **Departure scheduling patterns**
- **Airport congestion**
- **Route distance characteristics**

Taxi-out time emerged as the **strongest predictor of delay probability**.

---

# 🚀 Business Applications

Predictive delay models can help airlines:

- Identify high-risk flights early
- Improve ground operations coordination
- Optimize crew scheduling
- Improve passenger communication
- Reduce cascading operational disruptions

---

---

# 📌 Future Improvements

Potential extensions of this project include:

- Real-time delay prediction systems
- Integration with airline operations dashboards
- Explainable AI methods (SHAP values)
- Deployment using cloud infrastructure

---

# 👩‍💻 Authors

**Rashmika B**  
**Ekta Dubey**  
**Subrajeet Nayak**  
**Divya Bhatia**  
**Mohammed Saaliq**  
**Shreyas J**  
**under the guidance of Dr. Manisha Sharma**  
MBA, NMIMS Mumbai (2025-2027)

Predictive Analytics Project

---

# ⭐ If you found this project interesting

Feel free to **star the repository** and explore the analysis!

