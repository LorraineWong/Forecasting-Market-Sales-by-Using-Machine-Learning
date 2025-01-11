# WQD7004 Group Project - Forecasting Market Sales

## Project Overview

This project is part of the **WQD7004 Programming for Data Science** course. The objective is to predict supermarket sales trends, identify key factors influencing sales, and classify customer types (Normal or Member) using supervised machine learning techniques. The dataset is sourced from Kaggle and provides detailed transactional and demographic data from a supermarket.

---

## Objectives and Research Questions

### Objectives:
1. To classify customer types (Normal or Member) using supervised classification models.
2. To predict the total sales amount of individual transactions using regression models.
3. To compare and identify the best-performing model for both regression and classification tasks.
4. To evaluate model performance using key metric.

### Research Questions:
1. Which machine learning model provides the most accurate sales predictions?
2. What are the key factors influencing supermarket sales trends?
3. Which classification model (Random Forest, KNN, Decision Tree, XGBoost, LightGBM) performs best for predicting customer types?

---

## Dataset Details

- **Title**: Market Sales Data
- **Source**: [Kaggle - Market Sales Data](https://www.kaggle.com/datasets/willianoliveiragibin/market-sales-data/data)
- **Year**: 2024
- **Dimension**: 1000 rows × 9 columns
- **Structure**: Contains numerical and categorical data (e.g., `Invoice ID`, `Branch`, `City`, `Customer Type`, `Total`, etc.)
- **Purpose**: To analyze supermarket sales trends and forecast future sales.
- **Summary**: This dataset provides detailed transaction data from a supermarket, capturing customer demographics, product preferences, purchasing quantities, and sales-related financial details.

---

## Project Workflow

### 1. Data Preprocessing:
- **Steps**:
  - Handled missing values using mode and mean for imputation.
  - Removed unnecessary columns (e.g., `Invoice ID`).
  - Normalized and encoded categorical variables for machine learning compatibility.
  - Addressed outliers using interquartile range (IQR).

### 2. Exploratory Data Analysis (EDA):
- Gender and membership distributions were visualized using pie and bar charts.
- Analyzed sales distribution by `City`, `Branch`, and `Product Line`.
- Key insights:
  - Product line significantly impacts sales trends.
  - Membership and gender distributions influence customer purchasing behavior.

### 3. Model Development:
- **Regression Models**:
  - **Linear Regression**: Moderate performance.
  - **Random Forest Regression**: High R², reliable results.
  - **Gradient Boosting Regression**: Best performance with R² ~ 0.995.
- **Classification Models**:
  - **Random Forest**: Balanced performance, high accuracy.
  - **K-Nearest Neighbors (KNN)**: Best model for F1 Score and Recall.
  - **XGBoost & LightGBM**: Reliable alternatives with consistent performance.
  - **Decision Tree**: High interpretability but moderate accuracy.

### 4. Results and Insights:
- Gradient Boosting Regression outperformed other regression models.
- KNN excelled in customer classification with superior Recall and F1 Score.
- Important predictors for sales:
  - `City`, `Product Line`, and `Membership Type`.

### 5. Recommendations:
1. Use KNN for customer classification tasks requiring high sensitivity.
2. Implement Gradient Boosting Regression for accurate sales forecasting.
3. Expand the dataset and enhance feature engineering for improved model performance.

---

## Tools and Technologies

- **Programming Language**: R
- **Key Libraries**:
  - `dplyr`, `ggplot2`, `caret`, `randomForest`, `xgboost`, `e1071`, `readr`, `lightgbm`, `rpart`
- **Visualization**: Bar charts, pie charts, box plots.

---

## Deployment
- RPubs: [R Markdown](http://rpubs.com/Lorraine06/WQD7004-OCC3-Group-5)
- Presentation: [Video Link](https://drive.google.com/file/d/1LCjOU7npnWeIhCzIdAkXVJa7InX3Wn_f/view?usp=sharing)

---

## Author
- LOO LING YAN (23094683)
- XIAN ZHIYI (23122622)
- WONG YI TING (S2152880)
- CHU JING HAN (23116920)
- HAU JIA QI (17204762)

---

For more information or collaboration, feel free to raise an issue or contact me through GitHub.
