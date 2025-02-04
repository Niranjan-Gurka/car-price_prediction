# car-price_prediction
Here I performed data analysis on cars data with which I need to predict the price of car. I had trained a  ML model and tested the model.

# 🚗 Car Price Prediction using Regression Model

## 📌 Overview

This project aims to predict car prices based on various features like year of manufacture, present price, kilometers driven, fuel type, seller type, transmission type, and ownership history. We use Machine Learning **(Random Forest Regressor and Hyperparameter Tuning)** to build an accurate predictive model.


## 📂 Dataset

### The dataset used in this project (car data.csv) contains:

* Year - Year of manufacture

* Selling_Price - Price at which the car is being sold (Target variable)

* Present_Price - Showroom price of the car when new

* Kms_Driven - Number of kilometers driven
  
* Fuel_Type - Type of fuel used (Petrol/Diesel/CNG)

* Seller_Type - Type of seller (Dealer/Individual)

* Transmission - Manual or Automatic transmission

* Owner - Number of previous owners

## 🛠️ Technologies Used

- Python

- Pandas, NumPy (Data Manipulation & Cleaning)

- Matplotlib, Seaborn (Data Visualization)

- Scikit-Learn (Machine Learning Model)

## 📊 Steps Involved

## 1️⃣ Data Preprocessing

- Load dataset and check for missing values.

- Feature engineering: Add a column for No_of_Years (Current Year - Year).

- Convert categorical features into numerical using pd.get_dummies().

- Drop unnecessary columns.

## 2️⃣ Exploratory Data Analysis (EDA)

- Pairplot & Heatmap: To visualize feature relationships.

- Feature Importance: Using ExtraTreesRegressor to identify the most influential features.

## 3️⃣ Model Training

- Splitting data into training (70%) and testing (30%) sets.

- Training RandomForestRegressor.

- Performing Hyperparameter Tuning using RandomizedSearchCV.

## 4️⃣ Model Evaluation

- Prediction on test data.

## Error Metrics:

- Mean Absolute Error (MAE)

- Mean Squared Error (MSE)

- Root Mean Squared Error (RMSE)

- R² Score

## 📌 Results

- Best Parameters: {'n_estimators': 1000,
 'min_samples_split': 2,
 'min_samples_leaf': 1,
 'max_features': 'sqrt',
 'max_depth': 25}

- MAE: 0.89

- MSE: 4.01

- RMSE: 2.00

- R² Score: 0.8632

## 🏆 Key Takeaways:
- The model performs well with an R² Score close to 1, indicating good predictive power.

- Feature importance analysis helped in selecting relevant attributes.

- Hyperparameter tuning significantly improved model performance.

## 🚀 Future Improvements

- Try other regression models like XGBoost, Lasso, Ridge Regression.
  
- Deploy the model using Flask/Django for real-world use.
  
- Use more extensive datasets to enhance accuracy.
