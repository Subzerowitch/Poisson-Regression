# Poisson-Regression

**Bike Path Usage Analysis and Prediction**
  
This project aims to analyze the relationship between the number of bicyclists using different bike paths on the same day and predict the number of riders on one path based on the number on another path using Poisson Regression. The dataset used for this project contains information about the number of bicyclists on various bike paths in Montreal.

**Data Source**
  
  The dataset used for this project can be found on Kaggle at the following link: https://www.kaggle.com/datasets/pablomonleon/montreal-bike-lanes

**Exploratory Data Analysis (EDA)**
  
  The initial step involved loading the dataset and performing exploratory data analysis. Key steps in EDA include:

  -Plotting the number of bicyclists for each bike path over time to observe trends and correlations between paths.
  -Handling outliers in the dataset, imputing missing or incorrect values with sensible imputation based on surrounding data points.
  -Dropping columns with insufficient data and pre-processing the data for further analysis.
  -Correlation and Feature Selection
  -The correlation matrix was used to identify the bike paths most correlated with the target street ('Notre-Dame'). The top correlated streets were selected as features for building the prediction model.

**Correlation and Feature Selection**
  
  The correlation matrix was used to identify the bike paths most correlated with the target street ('Notre-Dame'). The top correlated streets were selected as features for building the prediction model.

  **Data Splitting**
  
  The data was split into training and testing sets for model building and evaluation. The training set was used to train the Poisson regression model, while the testing set was used to evaluate the model's performance.

**Poisson Regression Model**
  
  A Poisson regression model was selected for predicting the number of riders on the target street based on the number of riders on other correlated streets. Poisson regression is appropriate for modeling count data, such as the number of bicyclists.

**Model Evaluation**
  
  The model's performance was evaluated using mean squared error (MSE) and R-squared (R^2) score. The MSE measures the average squared difference between predicted and actual values, while the R^2 score indicates the proportion of variance in the target variable that is predictable from the input features.

**Model Visualization**
  
  A scatter plot was created to visualize the predicted values against the actual values. The plot helps to assess how well the Poisson regression model's predictions align with the actual data.

**Root Mean Squared Error (RMSE)**

  The root mean squared error (RMSE) was calculated as a measure of the model's prediction accuracy. The RMSE represents the standard deviation of the model's prediction errors.

**Conclusion**
  
  This project provides insights into the relationship between the number of bicyclists using different bike paths on the same day and demonstrates the use of a Poisson regression model to predict the number of riders on one path based on another. The model's performance can be further improved by exploring other regression techniques or incorporating additional features.

**Dependencies**

  pandas
  matplotlib
  scikit-learn
