# **Gold Price Analysis and Machine Learning Prediction**

---

## **Table of Contents**
- [Overview](#overview)
- [Project Structure](#project-structure)
- [Key Features](#key-features)
- [Results](#results)
- [Tools and Libraries](#tools-and-libraries)
- [How to Run](#how-to-run)

---

## **Overview**
This project analyzes historical gold price data over five years to identify trends, understand seasonal patterns, and develop a machine learning model to classify investment decisions as **Buy** or **Hold**. Through comprehensive data analysis, feature engineering, and predictive modeling, this project aims to provide actionable insights for investors.

---

## **Project Structure**
- **Data Analysis**:
  - Visualizations of historical gold price trends and seasonality.
  - Volatility and return analysis to assess risk.
- **Machine Learning**:
  - Feature engineering to extract meaningful insights.
  - Classification model to predict Buy/Hold investment signals.
  - Threshold tuning to optimize model performance.

---

## **Key Features**
1. **Descriptive Analysis**:
   - Seasonal and trend analysis using boxplots and moving averages.
   - Volatility analysis for risk assessment.
2. **Predictive Modeling**:
   - Random Forest Classifier trained on engineered features.
   - SMOTE applied to address class imbalance.
   - Threshold tuning to balance precision and recall for the **Buy** class.
3. **Visualization**:
   - Overlayed predictions on gold price charts to highlight Buy signals.

---

## **Results**
1. **Analysis Highlights**:
   - Identified seasonal trends in gold prices, showing consistent periodic fluctuations.
   - Rolling volatility provided insights into periods of high and low market risk.

2. **Model Performance**:
   - **Accuracy**: 76%
   - **Buy Class Recall**: 38%
   - **Buy Class Precision**: 28%
   - Effective identification of some **Buy** opportunities, though precision remains a challenge.

3. **Visual Insights**:
   - Clear representation of Buy signals on gold price charts aids interpretability for investors.

---

## **Tools and Libraries**
- **Python Libraries**:
  - `pandas`, `numpy` for data preprocessing and manipulation.
  - `matplotlib`, `seaborn` for data visualization.
  - `scikit-learn` for machine learning model development.
  - `imblearn` for handling class imbalance using SMOTE.

---

## **How to Run**
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Mattyb883/gold_analysis.git
   cd gold_analysis
