# Task3_Linear-Regression-House-Price-Prediction

## Overview  
This repository implements **Simple & Multiple Linear Regression** on a housing dataset, demonstrating predictive modeling, evaluation, and interpretation.  

## Objectives  
- Preprocess housing data (handling categorical variables, missing values).  
- Train and evaluate both simple (Area vs Price) and multiple regression models.  
- Interpret coefficients and metrics (MAE, MSE, R²).  
- Visualize relationships between features and target (Price).

## Tools & Technologies  
**Language**: Python  
**Environment**: Google Colab  
**Libraries Used**:
- Pandas (Data manipulation)  
- Scikit-learn (Regression models)  
- Matplotlib & Seaborn (Visualizations)

## Dataset  
- **Source**: [Kaggle Housing Dataset](https://www.kaggle.com/datasets/harishkumardatalab/housing-price-prediction)  
- **File**: `Housing.csv`  

**Key Features**:
- Numerical: `area`, `bedrooms`, `price`  
- Categorical: `furnishingstatus`, `mainroad` (one-hot encoded)

## Analysis Highlights  

### 1. Data Preprocessing  
- Checked for missing values using `isnull().sum()`  
- Converted categorical variables using one-hot encoding  
- Created a correlation heatmap to analyze feature relationships  

### 2. Statistical Analysis  
- Explored descriptive stats (mean, median) for `price`, `area`  
- Found `area` to be strongly correlated with `price`  

### 3. Key Visualizations  
#### Simple Regression:
- Scatter plot of `area` vs `price` with regression line  

#### Multiple Regression:
- Coefficient bar plot for feature importance  
- Residual analysis (actual vs predicted prices)

### 4. Model Evaluation  

| **Metric**     | **Simple Regression** | **Multiple Regression** |
|----------------|-----------------------|-------------------------|
| **MAE**        | 1,120,000             | 950,000                 |
| **R² Score**   | 0.32                  | 0.68                    |

---

## Key Findings  

### Area Impact  
- Positive linear relationship with price  
- R² = 0.32 in simple regression  

### Furnishing Status  
- Semi-furnished homes had a significant impact in multiple regression  

### Model Performance  
- Multiple regression (R² = 0.68) outperformed simple regression by **2.1×**

## Learning Outcomes  
- Applied **Scikit-learn** for regression modeling  
- Interpreted coefficients to explain feature impact  
- Visualized insights using heatmaps and regression plots  
- Compared model performance using **MAE, MSE, R²**

## Files  
- `Linear_Regression_Housing.ipynb` – Google Colab notebook  
- `Housing.csv` – Dataset 
