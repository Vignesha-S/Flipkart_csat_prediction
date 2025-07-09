# 📊 Flipkart CSAT Prediction

## 📁 Project Type

**Classification**

## 👤 Contribution

**Individual**

## 📝 Project Summary

This project aims to predict Customer Satisfaction (CSAT) scores based on customer service interaction data from Flipkart. In the competitive e-commerce landscape, customer satisfaction is key to retaining users and building brand loyalty. Flipkart's large-scale customer service data contains valuable insights into how various factors like issue types, response time, support channel, and supervisor/team affect customer satisfaction.

The dataset comprises customer service tickets with features such as issue type, sub-category, response time, agent shift, manager name, and more, alongside the target variable: `CSAT Score`. After detailed preprocessing, feature engineering, and handling class imbalance using SMOTE, we applied multiple machine learning models including:

* **Random Forest Classifier**
* **XGBoost Classifier**
* **LightGBM Classifier**

We evaluated models using **accuracy**, **precision**, **recall**, and **F1-score**, particularly focusing on performance for lower CSAT scores where business intervention is most needed.

Among all models, **LightGBM** with default parameters gave the highest accuracy (\~72.85%) but had poor recall for minority classes. Feature importance analysis revealed that **Supervisor**, **Sub-category**, and **Response Time** were the top contributors affecting CSAT predictions.

This model can guide Flipkart to:

* Prioritize reducing response time.
* Train specific agents or supervisors for certain issue types.
* Allocate better shifts or tenured agents to sensitive categories.

The insights and models created here can be integrated into Flipkart’s internal dashboards to help customer service managers track real-time performance and drive actionable improvements.

---

## 🔍 Problem Statement

To build a classification model that predicts customer satisfaction scores (CSAT) based on historical customer service data, enabling Flipkart to improve its service quality and increase customer retention.

---

## 💡 Business Context

In the highly competitive e-commerce space, delivering excellent customer service is crucial for sustaining growth and customer loyalty. Flipkart, as one of the largest e-commerce platforms, focuses on enhancing customer satisfaction to differentiate itself from competitors.

By analyzing customer support interactions and CSAT ratings, this project helps identify what drives good or poor satisfaction scores. This enables Flipkart to strategically allocate resources, reduce churn, and create a data-driven customer service strategy.

---

## 🧠 ML Models Used

* ✅ Random Forest
* ✅ XGBoost
* ✅ LightGBM

All models were evaluated using:

* **Accuracy**
* **Precision, Recall, F1-Score**
* **Class-wise performance**
* **Cross-validation**
* **Hyperparameter tuning (GridSearchCV)**

---

## 📌 Final Model Chosen

**LightGBM Classifier**
Achieved highest accuracy with best generalization, especially after considering runtime and interpretability.

---

## 🔎 Key Features Identified (Top 5 by Importance)

1. Supervisor
2. Sub-category
3. Response Time (mins)
4. Log of Response Time
5. Channel Name - Outcall

---
