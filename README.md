# Capstone-CarDekho

## Problem Statement:

### Objective:

Imagine you are working as a data scientist in Car Dheko, your aim is to enhance the customer experience and streamline the pricing process by leveraging machine learning. You need to create an accurate and user-friendly streamlit tool that predicts the prices of used cars based on various features. This tool should be deployed as an interactive web application for both customers and sales representatives to use seamlessly.

### Project Scope:

We have historical data on used car prices from CarDekho, including various features such as make, model, year, fuel type, transmission type, and other relevant attributes from different cities. Your task as a data scientist is to develop a machine learning model that can accurately predict the prices of used cars based on these features. The model should be integrated into a Streamlit-based web application to allow users to input car details and receive an estimated price instantly.

## Approach:

### 1.Data Processing:

a) Import and concatenate:
* Import all city’s dataset which is in unstructured format.
* Convert it into a  structured format.
* Add a new column named ‘City’ and assign values for all rows with the name of the respective city.
* Concatenate all datasets and make it as a single dataset.
  
b) Handling Missing Values: 
* Identify and fill or remove missing values in the dataset.
* For numerical columns, use techniques like mean, median, or mode imputation.
* For categorical columns, use mode imputation or create a new category for missing values.
  
c) Standardising Data Formats:
* Check for all data types and do the necessary steps to keep the data in the correct format.
* Eg. If a data point has string formats like 70 kms, then remove the unit ‘kms’ and change the data type from string to integers.
  
d) Encoding Categorical Variables:
* Convert categorical features into numerical values using encoding techniques.
* Use one-hot encoding for nominal categorical variables.
* Use label encoding or ordinal encoding for ordinal categorical variables.
  
e) Normalizing Numerical Features:
* Scale numerical features to a standard range, usually between 0 and 1.( For necessary algorithms)
* Apply techniques like Min-Max Scaling or Standard Scaling.
  
f) Removing Outliers:
* Identify and remove or cap outliers in the dataset to avoid skewing the model.
* Use IQR (Interquartile Range) method or Z-score analysis.

### 2. Exploratory Data Analysis (EDA):

a) Descriptive Statistics: 
* Calculate summary statistics to understand the distribution of data. i.e., Mean, median, mode, standard deviation, etc.
  
b) Data Visualization:
* Create visualizations to identify patterns and correlations.
* Use scatter plots, histograms, box plots, and correlation heatmaps.
  
c) Feature Selection:
* Identify important features that significantly impact the car prices.
* Use techniques like correlation analysis, feature importance from models, and domain knowledge.

### 3. Model Development:

a) Train-Test Split: 
* Split the dataset into training and testing sets to evaluate model performance.
* Common split ratios are 70-30 or 80-20.
  
b) Model Selection:
* Choose appropriate machine learning algorithms for price prediction.
* Linear Regression, Decision Trees, Random Forests, Gradient Boosting Machines, etc.
  
c) Model Training: 
* Train the selected models on the training dataset.
* Use cross-validation techniques to ensure robust performance.
  
d) Hyperparameter Tuning: 
* Optimize model parameters to improve performance.
* Use techniques like Grid Search or Random Search.

### 4. Model Evaluation:

a) Performance Metrics: 
* Evaluate model performance using relevant metrics.
* Mean Absolute Error (MAE), Mean Squared Error (MSE), R-squared.
  
b) Model Comparison:
* Compare different models based on evaluation metrics to select the best performing model.

### 5. Optimization:
   
a) Feature Engineering: 
* Create new features or modify existing ones to improve model performance.
* Use domain knowledge and exploratory data analysis insights.
  
b) Regularization:
* Apply regularization techniques to prevent overfitting.
* Lasso (L1) and Ridge (L2) regularization.

### 6. Deployment:
   
a) Streamlit Application: 
* Deploy the final model using Streamlit to create an interactive web application.
* Allow users to input car features and get real-time price predictions.
  
b) User Interface Design:
* Ensure the application is user-friendly and intuitive.
* Provide clear instructions and error handling.

## Results: 

* A functional and accurate machine learning model for predicting used car prices.
* Comprehensive analysis and visualizations of the dataset.
* Detailed documentation explaining the methodology, models, and results.
* An interactive Streamlit application for real-time price predictions based on user input.
