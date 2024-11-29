## Overview
This project focuses on predicting flight prices using machine learning techniques. The dataset comprises various features related to flights, including airlines, journey dates, source and destination cities, departure and arrival times, duration, number of stops, and additional information. The objective is to develop a predictive model that can accurately estimate flight prices based on these features.

## Requirements
To run this project, ensure you have the following libraries installed:
- **NumPy**: for numerical operations
- **Pandas**: for data manipulation and analysis
- **Matplotlib**: for data visualization
- **Seaborn**: for enhanced data visualization
- **Scikit-learn**: for machine learning algorithms and model evaluation

You can install these libraries using pip.

## Dataset
The project utilizes two datasets:
1. **Flight_Price_Train.xlsx**: This training dataset contains historical flight price data.
2. **Flight_Price_Test.xlsx**: This test dataset is used to evaluate the performance of the model.

## Insights
1. **Data Exploration**: Initial exploration reveals key statistics about the dataset, such as the average flight price, standard deviation, and distribution of various categorical features.
2. **Feature Engineering**: Significant features are extracted and transformed to improve model accuracy. This includes converting categorical variables into numerical formats and extracting additional features like journey day and month from the date of journey.
3. **Model Selection**: Several regression models are evaluated, including:
   - Linear Regression
   - Decision Tree Regressor
   - Random Forest Regressor

4. **Model Performance**: The effectiveness of each model is assessed using metrics such as Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared values.

## Model Steps Description

### 1. Data Loading
Load the training and test datasets using Pandas to facilitate data manipulation.

### 2. Data Exploration
Conduct basic exploration to understand the structure of the data:
- Check the first five records.
- Evaluate the shape of the dataset.
- Review statistical information (mean, standard deviation, minimum, maximum).
- Identify duplicates and null values.

### 3. Feature Engineering
Enhance the dataset by creating new features:
- Extract `Journey_day` and `Journey_month` from `Date_of_Journey`.
- Convert categorical variables into numerical formats using encoding techniques.

### 4. Data Splitting
Divide the training dataset into training and validation sets to evaluate model performance during training.

### 5. Model Training
Train multiple regression models on the training dataset to find the best-performing algorithm.

### 6. Model Evaluation
Assess the trained model on the validation set using appropriate metrics to gauge its performance.

### 7. Predictions on Test Data
Utilize the trained model to predict flight prices on the test dataset, allowing for evaluation against known outcomes.
