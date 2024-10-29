# Laptop Price Prediction
This is the project i did in Jupyter Notebook (Python).

## Problem Statement

With the growing variety of laptop models and specifications available in the market, consumers often struggle to make informed purchasing decisions based on price. 
This project aims to develop a predictive model that accurately estimates laptop prices based on various features such as RAM, weight, brand, and operating system.

## Purpose

The primary purpose of this project is to leverage data analysis and machine learning techniques to create a model that predicts laptop prices, providing valuable insights
to consumers and retailers alike. This model will help consumers make informed choices and assist retailers in setting competitive prices.

## Importance

- Consumer Empowerment: Accurate price predictions enable consumers to understand the market better and avoid overpaying for laptops.
- Business Strategy: Retailers can utilize pricing models to optimize their pricing strategies, manage inventory efficiently, and improve customer satisfaction.
- Market Insights: Understanding the factors influencing laptop prices can help manufacturers and marketers position their products more effectively.
  
## Objectives

- Data Collection: Gather a comprehensive dataset of laptops, including various specifications and prices.
- Data Preprocessing: Clean and prepare the data for analysis by handling missing values, detecting outliers, and scaling features.
- Model Development: Train and evaluate multiple regression models (e.g., Linear Regression, Ridge Regression, Random Forest) to find the best-performing one.
- Model Evaluation: Compare the models based on performance metrics such as R-squared, Mean Absolute Error, and Mean Squared Error.
- Insights Generation: Analyze the model outcomes to derive key insights regarding laptop pricing trends.
  
## Steps Involved

### Data Collection:

Gather data from various sources, such as online retailers and databases. Ensure that the dataset includes relevant features like RAM, weight, brand, and price.

### Data Preprocessing:

- Handling Missing Values: Identify and fill in or remove missing data to maintain dataset integrity.
- Outlier Detection: Use statistical methods and visualizations to identify and manage outliers that may skew results.
- Feature Encoding: Convert categorical features into numerical formats suitable for machine learning algorithms.
- Data Normalization: Scale features using StandardScaler to ensure uniformity across different scales.
  
### Model Development:

Split the dataset into training and testing sets (80/20) using train_test_split().
Fit various regression models (Linear Regression, Ridge Regression, Random Forest, etc.) to the training data.

### Model Evaluation:

Assess model performance using metrics such as R-squared, Mean Absolute Error, Mean Squared Error, and Root Mean Squared Error.

### Insights Generation:

Analyze model results to identify trends and correlations between features (e.g., RAM vs. price) and generate actionable insights.


## Regression models


### 1. Linear Regression


Description: Linear Regression is one of the simplest regression techniques, which assumes a linear relationship between the independent variables (features) and the dependent variable (price). It estimates the coefficients that minimize the difference between the predicted and actual values.

Performance Metrics:

- R-squared Score: 0.672
- Mean Squared Error (MSE): 0.132
- Mean Absolute Error (MAE): 0.279
- Root Mean Squared Error (RMSE): 0.363
  
Insights: The R-squared score indicates that approximately 67.2% of the variance in laptop prices can be explained by the features used in the model. While it provides a baseline, the performance could be improved with more complex models.



### 2. Ridge Regression

Description: Ridge Regression is a type of linear regression that includes L2 regularization, which helps prevent overfitting by adding a penalty for large coefficients. This is particularly useful in cases where there are many features or multicollinearity.

Performance Metrics:

- R-squared Score: 0.671
- Mean Squared Error (MSE): 0.132
- Mean Absolute Error (MAE): 0.279
- Root Mean Squared Error (RMSE): 0.364

  
Insights: The performance metrics for Ridge Regression are similar to those of Linear Regression, with a slightly lower R-squared score. This suggests that while regularization helps in certain contexts, it may not significantly enhance performance in this dataset.

### 3. Random Forest Regression
Description: Random Forest Regression is an ensemble learning method that uses multiple decision trees to make predictions. It aggregates the predictions from various trees to improve accuracy and control overfitting.

Performance Metrics:

- R-squared Score: 0.906
- Mean Squared Error (MSE): 0.037
- Mean Absolute Error (MAE): 0.152
- Root Mean Squared Error (RMSE): 0.194


Insights: Random Forest Regression outperformed the other models, with an R-squared score of 90.6%, indicating that it explains a large portion of the variance in laptop prices. Its low error metrics reflect its robustness and effectiveness in capturing complex relationships in the data.

### 4. Support Vector Machine (SVM) Regression


Description: Support Vector Machine Regression (SVR) is based on the principles of support vector machines and is effective for high-dimensional spaces. It attempts to find a hyperplane that best separates the data points, accommodating non-linear relationships through the kernel trick.

Performance Metrics:

- R-squared Score: 0.893
- Mean Squared Error (MSE): 0.042
- Mean Absolute Error (MAE): 0.154
- Root Mean Squared Error (RMSE): 0.207

  
Insights: With an R-squared score of 89.3%, SVR shows strong performance in predicting laptop prices. Its metrics suggest it captures complex relationships well but slightly lags behind Random Forest in performance.


### 5. AdaBoost Regression

Description: AdaBoost Regression is an ensemble method that combines the predictions from multiple weak learners (often decision trees) to improve accuracy. It focuses on misclassified data points to adjust the model iteratively.

Performance Metrics:

- R-squared Score: 0.840
- Mean Squared Error (MSE): 0.064
- Mean Absolute Error (MAE): 0.202
- Root Mean Squared Error (RMSE): 0.254

  
Insights: The performance metrics for AdaBoost Regression indicate good predictive power, with an R-squared score of 84.0%. Although it does not outperform Random Forest, it still provides reliable predictions and is useful in capturing various patterns in the data.


## Visuals and Key Insights

### Scatter Plot of RAM vs. Price:

Shows a positive correlation between RAM and laptop prices, with most laptops clustering around lower RAM values.

### Histogram of Weight Distribution:

Reveals common weight categories, indicating the prevalence of certain laptop types (e.g., ultrabooks vs. gaming laptops).

### Bar Chart of Laptop Brands:

Displays the frequency of laptops from various brands, highlighting market representation.

### Average Prices by Operating System:

Illustrates price variations across different operating systems, informing consumers about cost differences.

### Correlation Matrix:

Summarizes pairwise correlations among features, indicating the relationships and potential multicollinearity between them.

![image](https://github.com/user-attachments/assets/fe867f95-5f27-4316-80a3-740d58e27007)


## Technical Skills

- Data Analysis: Proficiency in Python and libraries such as Pandas, NumPy, and Matplotlib for data manipulation and visualization.
- Machine Learning: Knowledge of regression techniques and experience with Scikit-learn for model building and evaluation.
- Data Preprocessing: Skills in handling missing data, outlier detection, and feature engineering.
- Statistical Analysis: Ability to interpret performance metrics and assess model efficacy.
  
## Soft Skills

- Problem Solving: Critical thinking to analyze data and identify pricing trends.
- Communication: Effectively presenting findings and insights to stakeholders.
- Adaptability: Flexibility in learning new tools and techniques as needed during the project.
- Collaboration: Working effectively with team members or stakeholders to gather requirements and present results.
  
## Conclusion

The laptop price prediction project illustrates the significant role of data analytics and machine learning in understanding
market dynamics and consumer behavior. By accurately predicting laptop prices based on key features, this project not only aids
consumers in making informed choices but also supports retailers in strategic pricing decisions. The findings underscore the importance 
of various laptop specifications, particularly RAM, in influencing prices while also highlighting the effectiveness of Random Forest regression 
as a predictive model. In a rapidly evolving tech landscape, such insights contribute to better decision-making, enhance customer satisfaction, and foster business growth.
