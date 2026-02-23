# Insurance Claims Analysis & Prediction

## Project Overview
**Insurance Claims Analysis & Prediction** is a data analytics and machine learning project that analyzes insurance policyholder data, identifies key factors influencing claim amounts, and builds predictive models to estimate future claims. This project provides actionable business insights to help insurance companies make data-driven decisions on risk assessment, policy pricing, and preventive strategies.

## Key Features of the Project
- **Data Cleaning & Preprocessing:** Handle missing values, encode categorical variables, and prepare the dataset for modeling.  
- **Exploratory Data Analysis (EDA):** Visualize the distribution of claims, explore relationships between features and claim amounts, and identify trends.  
- **Predictive Modeling:** Implement Linear Regression and Random Forest Regressor to predict insurance claim amounts.  
- **Model Evaluation:** Compare models using RMSE, R², and MAE; Random Forest emerges as the best-performing model.  
- **Feature Importance & Insights:** Identify which factors (e.g., smoker status, age, BMI, region) have the largest impact on claims.  
- **Visualization & Reporting:** Generate plots for distributions, correlations, and feature importance, saved for documentation and presentations.

## Dataset
The dataset includes the following columns:  
- `Id` – Unique identifier  
- `age` – Age of the policyholder  
- `gender` – Gender (male/female)  
- `bmi` – Body Mass Index  
- `bloodpressure` – Blood pressure measurement  
- `diabetic` – Diabetes status (yes/no)  
- `children` – Number of children covered  
- `smoker` – Smoker status (yes/no)  
- `region` – Geographic region  
- `claim` – Insurance claim amount (target variable)

## Steps Followed

1. **Data Cleaning & Missing Values:** Fill missing numeric and categorical values.  
2. **Exploratory Data Analysis (EDA):** Plot distributions, boxplots, and correlation heatmaps.  
3. **Feature Engineering:** Encode categorical variables using one-hot encoding.  
4. **Train/Test Split:** Split dataset into 80% training and 20% testing.  
5. **Modeling:** Train Linear Regression and Random Forest Regressor models.  
6. **Evaluation:** Evaluate models using RMSE, R², and MAE.  
7. **Business Insights:** Analyze feature importance and derive actionable recommendations.

## Model Performance
| Model | RMSE | R² | MAE |
|-------|------|----|-----|
| Linear Regression | 6538.77 | 0.74 | 4891.71 |
| Random Forest | 5421.31 | 0.82 | 4017.58 |

---

## Feature Importance (Random Forest)
Top predictors influencing insurance claim amounts:  
1. **Smoker status** – smokers consistently have higher claims.  
2. **Age** – older policyholders tend to have higher claims.  
3. **BMI** – higher BMI is associated with increased claim amounts.  
4. **Blood pressure** – elevated blood pressure contributes to risk.  
5. **Region differences** – certain regions may have systematically higher claims.

## Business Insights & Recommendations
1. **Risk-based Pricing:** Higher premiums for smokers, older clients, and high-BMI individuals can balance claim costs.  
2. **Preventive Programs:** Encourage healthier lifestyles (weight management, blood pressure control) to reduce claims.  
3. **Regional Analysis:** Consider regional pricing adjustments based on claims patterns.  
4. **Stakeholder Next Steps:** Use Random Forest predictions for risk scoring and policy pricing; monitor feature importance over time as demographics and behaviors evolve.

## Technologies Used
- Python  
- Pandas & NumPy – Data manipulation and preprocessing  
- Matplotlib & Seaborn – Visualization  
- Scikit-learn – Machine learning models (Linear Regression, Random Forest)  
- Jupyter Notebook – EDA and interactive exploration

## Conclusion
Random Forest outperforms Linear Regression for predicting insurance claims, capturing non-linear relationships in features like smoker status, age, and BMI. Feature importance provides actionable insights for insurance companies to optimize risk assessment, pricing strategies, and preventive health initiatives.
