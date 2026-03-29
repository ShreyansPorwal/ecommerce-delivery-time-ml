# E-Commerce Delivery Time Prediction

## Overview

Built an end-to-end machine learning system to predict e-commerce delivery times using structured logistics and product data.

The project focuses on identifying key factors that impact delivery performance and deploying a model capable of making real-time predictions.

---

## Key Contributions

* Developed a full ML pipeline from data preprocessing → modeling → evaluation → deployment
* Reduced prediction error (MAE) by ~30% compared to baseline
* Identified **product weight and cost** as major drivers of delivery delays
* Built and deployed a **Flask API** for real-time inference
* Created visualizations to analyze feature importance and model behavior

---

## Dataset

* ~11,000 shipment records

* Features include:

  * Warehouse block
  * Shipment mode
  * Product cost
  * Discount offered
  * Product weight
  * Customer inquiries

* Target:

  * Delivery time / delay outcome

---

## Methodology

### 1. Data Processing

* Cleaned and handled missing values
* Encoded categorical variables
* Scaled numerical features
* Performed feature engineering on cost and weight

### 2. Exploratory Data Analysis

* Correlation analysis to identify key predictors
* Distribution analysis of delivery delays
* Visualization of relationships between features and target

---

## Modeling

### Models Used

* Decision Tree
* Random Forest (best performing)
* Logistic Regression

### Model Selection

* Used cross-validation for evaluation
* Compared models using:

  * MAE (Mean Absolute Error)
  * Accuracy

### Final Model

* **Random Forest**
* Best balance of accuracy and generalization

---

## Results

* Reduced MAE by ~30% from baseline
* Achieved ~92% accuracy on classification task
* Strong generalization across validation data

---

## Deployment

* Built a **Flask API** for serving predictions
* Allows real-time input of shipment features
* Returns predicted delivery time / delay outcome

---

## Tech Stack

* Python
* Scikit-learn
* Pandas, NumPy
* Matplotlib / Seaborn
* Flask
* Google Cloud Platform (GCP)

---

## Key Insights

* Heavier products significantly increase delivery delays
* Product cost correlates with shipping priority and performance
* Customer interaction patterns influence delivery outcomes

---

## Future Improvements

* Hyperparameter tuning with Grid/Random Search
* Ensemble methods (XGBoost, LightGBM)
* Real-time streaming data integration
* Frontend dashboard for predictions
