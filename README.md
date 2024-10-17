# Telematics Data Analysis for Insurance

## Description

This project aims to predict insurance claim amounts and classify policyholders based on their risk level, using telematics and contract data. The project applies machine learning and econometric methods to develop predictive models that optimize risk management and pricing strategies in the insurance sector.

## Objectives

- **Claim Amount Prediction**: Use regression techniques to estimate claim amounts.
- **High-Risk Policyholder Classification**: Identify high-risk policyholders to better target pricing and preventive actions.
- **Understanding Key Variables**: Analyze the variables that have the most influence on claim amounts and driving behaviors.

## Datasets

The project uses three main data sources:
1. **Claims Data (DB_SIN.txt)**: Contains detailed information on insurance claims.
2. **Contract Data (DB_CNT.xlsx)**: Includes data on insurance contracts, with variables such as the insured's age, credit score, and contract duration.
3. **Telematics Data (DB_TELEMATICS.csv)**: Contains telematics data reflecting driving behavior.

## Approaches Used

### 1. **Data Preprocessing**
- Data cleaning and standardization.
- Handling missing values and outliers.
- Encoding categorical variables and normalizing the data.

### 2. **Exploratory Data Analysis (EDA)**
- Univariate and multivariate analysis of key variables.
- Exploration of driving behaviors and claims with graphical visualizations (histograms, boxplots).

### 3. **Predictive Models**
- **Ridge Regression**: Used to predict claim amounts with regularization to limit overfitting.
- **Random Forest**: Ensemble model used for both prediction and classification, capturing complex interactions between variables.
- **XGBoost**: A powerful boosting algorithm used to refine predictions.

### 4. **Econometric Analysis**
- Multiple linear regression model to understand the factors influencing claim amounts.
- Polynomial model to capture nonlinear relationships between predictors.

## Results

- The **Random Forest model** provided the best performance in predicting claim amounts, with an **RMSE** of 1849.27.
- Variables such as **Years.noclaims** (years without a claim) and **Credit_score_cat_Low** (low credit score) were identified as key predictors of claim amounts.
- The **policyholder classification** reached a moderate accuracy with an AUC of 0.67, suggesting room for improvement in risk management.

## Limitations and Recommendations

- **Multicollinearity**: Variables like **Car.use** and **Region** exhibited multicollinearity, which could affect model precision.
- **Model Improvement**: Further regularization techniques like Lasso regression and exploring nonlinear models such as neural networks could enhance results.
- **Data Enrichment**: Incorporating additional data, especially related to driving behavior, could improve predictions.

## Conclusion

This project highlights the importance of data analysis in optimizing risk management in the insurance sector. Machine learning methods, combined with econometric approaches, provide a deeper understanding of the factors driving claims while enabling more accurate pricing strategies.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

