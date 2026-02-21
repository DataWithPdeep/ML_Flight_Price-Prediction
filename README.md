#  Flight Price Prediction System

This project is a **Machine Learning based Flight Price Prediction system** developed using Python.  
It predicts airline ticket prices based on journey details such as airline, source, destination, stops, duration, and timings.

---

# Project Objective

- Understand the factors affecting flight prices
- Perform extensive **EDA & Feature Engineering**
- Build and compare multiple **Regression models**
- Select the best-performing model for prediction
- Save the trained model for deployment

---

# Dataset Information

- **Training Data:** `Data_Train.xlsx`
- **Test Data:** `Test_set.xlsx`
- Columns include:
  - Airline
  - Source
  - Destination
  - Total Stops
  - Date of Journey
  - Departure & Arrival Time
  - Duration
  - Price (Target Variable)

---

# Tech Stack & Libraries

- Python 
- NumPy & Pandas
- Matplotlib & Seaborn
- Scikit-learn
- CatBoost
- XGBoost
- LightGBM
- Random Forest
- Extra Trees Regressor

---

# Exploratory Data Analysis (EDA)

- Missing value handling
- Duplicate removal
- Price distribution analysis
- Airline vs Price
- Source & Destination vs Price
- Stops vs Price
- Correlation heatmap

---

# Feature Engineering

- Extracted **Day & Month** from Date_of_Journey
- Extracted **Hour & Minute** from Departure & Arrival time
- Split **Duration** into hours and minutes
- Handled inconsistent destination names (New Delhi → Delhi)
- Label Encoding for `Total_Stops`
- One-Hot Encoding for:
  - Airline
  - Source
  - Destination

---

# Models Used

- Extra Trees Regressor
- Random Forest Regressor
- RandomizedSearchCV (Hyperparameter Tuning)
- CatBoost Regressor ✅
- LightGBM Regressor
- XGBoost Regressor

---

# Model Evaluation Metrics

- R² Score
- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)

---

# Best Performing Model

**CatBoost Regressor** showed strong performance without extensive preprocessing and was selected for deployment.

---

# Saved Files

- `model.pkl` → Trained CatBoost model
- `deploy_df.csv` → Cleaned dataset for deployment
- Encoded & engineered features ready for prediction

---

