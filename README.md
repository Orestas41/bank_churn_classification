<h1 align='center'>Bank Churn Classification</h1>
<h3 align='center'>Orestas Dulinskas</h3>
<h4 align='center'>January 2024</h4>

## Background

This data science project aims to leverage a comprehensive banking dataset to predict customer churn. Churn, in this context, refers to customers leaving the bank during a specified period. The dataset includes various features such as customer demographics (e.g., age, gender, country), financial information (credit score, balance), and banking-related attributes (tenure, product usage). Through rigorous analysis and machine learning modeling, the project seeks to identify key factors influencing customer churn, ultimately providing insights that can inform strategic retention efforts and enhance customer satisfaction.

## Objective

The primary objective of this project is to develop a predictive model that accurately anticipates customer churn based on the provided dataset. By employing machine learning algorithms and statistical analysis, the project aims to uncover patterns and relationships within the data. Specifically, it intends to answer questions such as:

Which features strongly correlate with customer churn? Are there demographic factors (e.g., age, gender) that significantly impact churn rates? Can machine learning models accurately predict which customers are more likely to churn? The overarching goal is to empower the bank with actionable insights to proactively address potential churners, optimize customer retention strategies, and improve overall customer satisfaction.

## Data

The dataset consists of the following features:

* Customer ID (unused variable)
* Credit score
* Country
* Gender
* Age
* Tenure
* Balance
* Products number
* Credit card usage
* Active membership status
* Estimated salary
* Churn (target variable: 1 if the customer has left the bank, 0 otherwise)

The dataset provides a comprehensive view of customer behavior and attributes, offering the necessary information for building a robust predictive model. Initial exploration will involve assessing data quality, identifying patterns, and gaining insights into the factors influencing customer churn. The dataset will be split into training and testing sets for model development and evaluation. The project will follow a systematic approach to data preprocessing, model selection, and performance evaluation to achieve the defined objectives.

## EDA Summary

Upon analyzing categorical features of the dataset, it becomes evident that the variables `IsActiveMember`, `Tenure`, and `Gender` exhibit comparable distributions, suggesting potential interdependencies or correlations among them. This similarity may indicate that the tenure of a customer, their gender, and their active membership status might influence each other or share common patterns within the dataset. On the other hand, the variables `HasCrCard`, `NumOfProducts`, and `Geography` showcase distinct distributions, implying diverse patterns or characteristics associated with these features. The dissimilarity in distributions for `HasCrCard` suggests variations in the prevalence of credit card ownership among customers, while `NumOfProducts` indicates diverse product usage patterns. Additionally, `Geography`, representing the customer's location, manifests differences, suggesting that regional factors could play a significant role in shaping customer behaviors or preferences within the dataset.

The examination of the Continuous features of the dataset reveals distinctive characteristics in the distribution of variables. Notably, the `balance` variable displays a considerable number of 0 values, resulting in a leftward skewness, indicating a concentration of customers with zero balances. This concentration could signify a specific subgroup within the dataset, possibly those with no account activity or certain restrictions. Moreover, the distributions of the remaining variables also exhibit skewness, either to the left or the right, implying asymmetry in their patterns. Interestingly, both the Exited and Not Exited classes share similar distributions for all variables, suggesting that the factors influencing customer exit decisions are distributed similarly across the dataset.
