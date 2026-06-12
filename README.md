# 🍔 Food Delivery Time Prediction – Tech Analytics Hackathon

## 📌 Project Overview

This repository contains the complete submission for the **IIT-BHU Tech Analytics Hackathon** by **Team Syntax Error**. The project focuses on predicting food delivery time using Machine Learning and Deep Learning techniques while analyzing the impact of feature richness on model performance.

A comparative study was conducted using two datasets:

1. **Dataset Provided by Organisers (Primary Dataset)** – Used for all official experimentation and evaluation.
2. **Dataset with Full Features (Secondary Dataset)** – Used only to understand performance differences observed in public implementations.

The study demonstrates how contextual features such as weather, traffic, city information, and order timing significantly improve prediction accuracy.

---

## 👨‍💻 Team Information

**Team Name:** Syntax Error

### Team Members

| Sr. No. | Name | Role |
|----------|----------|----------|
| 1 | Abhinandan Pakhare | Team Member |
| 2 | Animesh Kewale | Team Member |
| 3 | Rajat Kantode | Team Member |

---

## 🏆 Hackathon Details

**Event:** IIT-BHU Tech Analytics Hackathon 2026

**Project Title:** Food Delivery Time Prediction

**Submission Categories:**
- Machine OR Deep Learning Models
- Data Analytics & Visualization (Power BI)


---

## 📂 Repository Structure

```text
IIT-BHU-Tech-Analytics/
│
├── SyntaxError_Report/
│   └── Food_Delivery_TechAnalytics.pbix
│
└── SyntaxError_ModelRound/
    │
    ├── README.md
    │
    ├── Dataset Provided by Organiser/
    │   ├── train.xlsx
    │   ├── EDA_New_Data_Train_fdt.ipynb
    │   ├── FineTunned_XgBoost.ipynb
    │   ├── Newdata_ML_Model.ipynb
    │   └── Newdata_DL_Model.ipynb
    │
    └── Dataset with Full Features/
        ├── Food Delivery Time Prediction Case Study.xlsx
        ├── FULL_EDA_Report.ipynb
        ├── ML_Model_without_FE.ipynb
        ├── ML_Model_with_Feature_Eng.ipynb
        ├── ML_model_tune.ipynb
        ├── DL_model.ipynb
        ├── DL_model_(3_input_para).ipynb
        └── ML_Model_(3_input_para).ipynb
```

---

## 🎯 Problem Statement

Predict the delivery time of food orders based on available order, restaurant, delivery partner, and location information.

The challenge was to build accurate regression models capable of estimating delivery duration while understanding the factors influencing prediction performance.

---

## 📊 Dataset Analysis

### 1️⃣ Dataset Provided by Organiser (Primary Dataset)

This dataset served as the official competition dataset and was used for all primary experiments.

### Features

* Delivery Person Age
* Delivery Person Rating
* Restaurant Latitude
* Restaurant Longitude
* Delivery Location Latitude
* Delivery Location Longitude
* Type of Order
* Type of Vehicle

### Target Variable

```text
Time_taken(min)
```

### Characteristics

* Basic delivery metadata
* Geographical information
* Limited contextual information
* No traffic conditions
* No weather information
* No order timing details

---

## 🔬 Exploratory Data Analysis

The following analyses were performed:

* Missing value analysis
* Distribution analysis
* Correlation analysis
* Geographic distance exploration
* Delivery time distribution
* Feature importance evaluation
* Outlier detection

Notebook:

```text
EDA_New_Data_Train_fdt.ipynb
```

---

## 🤖 Machine Learning Models

### Models Evaluated

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor
* XGBoost Regressor
* Hyperparameter Tuned XGBoost

### Best Model

| Metric   | Value                       |
| -------- | --------------------------- |
| Model    | Gradient Boosting Regressor |
| R² Score | 0.406                       |
| RMSE     | ±7.23 Minutes               |

### Observation

The organiser dataset produced relatively low R² scores due to limited contextual information, making accurate delivery time prediction challenging.

---

## 🧠 Deep Learning Models

Deep Learning approaches were also evaluated to determine whether neural networks could improve performance.

Models explored:

* Feed Forward Neural Networks
* Dense Neural Networks
* Multi-input Neural Network Architectures

Notebook:

```text
Newdata_DL_Model.ipynb
```

---

## 📈 Dataset with Full Features (Secondary Dataset)

A secondary dataset containing additional contextual information was used for comparative analysis.

### Additional Features

* Order Date
* Time Ordered
* Time Picked
* Weather Conditions
* Road Traffic Density
* Vehicle Condition
* Multiple Deliveries
* Festival Indicator
* City

### Benefits

These features provide:

* Temporal Context
* Traffic Information
* Environmental Conditions
* Operational Logistics

---

## 🚀 Advanced Modelling

### Feature Engineering

Performed:

* Time Feature Extraction
* Distance Calculations
* Categorical Encoding
* Traffic-Based Features
* Weather-Based Features

Notebook:

```text
ML_Model_with_Feature_Eng.ipynb
```

### Hyperparameter Tuning

Implemented:

* Grid Search
* Cross Validation
* XGBoost Optimization

Notebook:

```text
ML_model_tune.ipynb
```

---

## 🏆 Best Performance Achieved

### Secondary Dataset

| Metric   | Value                   |
| -------- | ----------------------- |
| Model    | Tuned XGBoost Regressor |
| R² Score | 0.8313                  |
| RMSE     | 3.88 Minutes            |

---

## 📊 Comparative Results

| Factor               | Organiser Dataset | Full Feature Dataset |
| -------------------- | ----------------- | -------------------- |
| Contextual Features  | Low               | High                 |
| Weather Data         | ❌                 | ✅                    |
| Traffic Data         | ❌                 | ✅                    |
| Temporal Information | ❌                 | ✅                    |
| Feature Richness     | Limited           | Extensive            |
| Best R² Score        | 0.406             | 0.831                |
| RMSE                 | 7.23 min          | 3.88 min             |

---

## 💡 Key Findings

### Organiser Dataset

* Limited contextual information restricts prediction capability.
* Most models achieved R² between 0.30–0.40.
* Model performance is constrained by available features rather than algorithm selection.

### Full Feature Dataset

* Significant improvement observed after adding contextual variables.
* Weather and traffic information strongly influence delivery time.
* Feature engineering substantially boosts performance.

---

## 📊 Power BI Dashboard

The repository includes a Power BI dashboard:

```text
Food_Delivery_TechAnalytics.pbix
```

Dashboard Features:

* Delivery Time Analysis
* Performance Metrics
* Geographic Insights
* Feature Impact Analysis
* Interactive Visualizations

---

## 🛠 Technologies Used

### Programming

* Python

### Libraries

* Pandas
* NumPy
* Scikit-Learn
* XGBoost
* TensorFlow / Keras
* Matplotlib
* Seaborn

### Visualization

* Power BI

---

## ▶️ How to Run

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Open Jupyter Notebook

```bash
jupyter notebook
```

### Run Notebooks

For Organiser Dataset:

```text
EDA_New_Data_Train_fdt.ipynb
Newdata_ML_Model.ipynb
Newdata_DL_Model.ipynb
```

For Full Feature Dataset:

```text
FULL_EDA_Report.ipynb
ML_Model_with_Feature_Eng.ipynb
ML_model_tune.ipynb
DL_model.ipynb
```

---

## 📌 Final Clarification

* The organiser-provided dataset was treated as the official competition dataset.
* All primary conclusions and evaluations are based on the organiser dataset.
* The full-feature dataset was used only to investigate performance discrepancies observed in public implementations.
* This comparison highlights the critical role of contextual features in real-world delivery time prediction systems.

---

## 📜 Conclusion

This project demonstrates that **feature quality is often more important than model complexity**. While advanced algorithms can improve performance, the availability of contextual information such as traffic, weather, and order timing has a significantly larger impact on prediction accuracy.

The study provides valuable insights into practical machine learning deployment for logistics and food delivery systems.

---

**Team Syntax Error**
🏆 IIT-BHU Tech Analytics Hackathon Submission 2026
