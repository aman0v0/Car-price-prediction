# Car Price Prediction

## Overview
This project predicts the price of a car based on various features using **Machine Learning**. The dataset contains multiple attributes like fuel type, seller type, transmission, and more, which help in determining the price of a car.

## Features
- **Data Preprocessing:** Cleaning and transforming raw data for analysis.
- **Exploratory Data Analysis (EDA):** Visualizing trends and relationships between features.
- **Model Training:** Implementing **Linear Regression** and **Lasso Regression**.
- **Model Evaluation:** Measuring performance using metrics like **Mean Absolute Error (MAE), Mean Squared Error (MSE), and R-squared (R²) Score**.

## Dataset
The dataset used is **car data.csv**, sourced from Kaggle: [Vehicle Dataset from CarDekho](https://www.kaggle.com/datasets/nehalbirla/vehicle-dataset-from-cardekho).

### Features in the dataset:
- **Car_Name**: Name of the car
- **Year**: Manufacturing year
- **Selling_Price**: Price at which the car is being sold
- **Present_Price**: Current ex-showroom price of the car
- **Kms_Driven**: Distance driven in kilometers
- **Fuel_Type**: Type of fuel (Petrol/Diesel/CNG)
- **Seller_Type**: Individual or Dealer
- **Transmission**: Manual or Automatic
- **Owner**: Number of previous owners

## Installation & Usage
1. Clone the repository:
   ```sh
   git clone https://github.com/aman0v0/Car-price-prediction.git
   cd Car-Price-Prediction
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the script:
   ```sh
   python car_price_prediction.py
   ```

## Model Training
- **Splitting the dataset:**
  ```python
  X_train, X_test, Y_train, Y_test = train_test_split(X, Y, test_size=0.2, random_state=2)
  ```
- **Applying Linear Regression:**
  ```python
  model = LinearRegression()
  model.fit(X_train, Y_train)
  ```
- **Applying Lasso Regression:**
  ```python
  model = Lasso()
  model.fit(X_train, Y_train)
  ```

## Evaluation Metrics
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **R-squared Score (R²)**

## Visualizations
The project includes **Seaborn and Matplotlib visualizations** to explore data insights, including:
- Correlation heatmaps
- Pair plots
- Actual vs Predicted price scatter plots

## License
This project is licensed under the **MIT License**.

## Author
Developed by **Mohammed Aman (GitHub: [aman0v0](https://github.com/aman0v0))**.

