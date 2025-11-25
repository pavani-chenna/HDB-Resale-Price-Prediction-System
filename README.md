# Singapore HDB Resale Price Prediction

This project predicts Singapore HDB resale flat prices using machine learning (Random Forest Regressor). It includes a Streamlit web application where users can input flat details and get an estimated resale price.

## Features
- Predict resale price based on Town, Flat type, Floor area (sqm), Storey range, Remaining lease years, Transaction year.
- Random Forest Regressor for accurate predictions.
- Label Encoding for categorical variables.
- Preprocessing and feature engineering for better model performance.

## Files in this Repository
- `app.py` – Streamlit web application for resale price prediction.
- `random_forest_model.pkl` – Trained Random Forest model.
- `encoded_town.pkl` – Label encoder for town.
- `flat_type_encoded.pkl` – Label encoder for flat type.



## Run the Streamlit App
- streamlit run app.py


## How to Use the App

1. Select the **Town** and **Flat Type** from dropdown menus.  
2. Input numeric values for **Floor Area (sqm)**, **Remaining Lease (years)**, and **Transaction Year**.  
3. Enter **Storey Range** in the format `X TO Y` (e.g., `10 TO 12`).  
4. Click **Predict Resale Price** to see the estimated resale price.

## Model Details

- **Algorithm:** Random Forest Regressor  
- **Evaluation Metrics:**  
  - Mean Absolute Error (MAE)  
  - Mean Squared Error (MSE)  
  - Root Mean Squared Error (RMSE)  
  - R² Score  
- **Feature Engineering:**  
  - Converted categorical variables using Label Encoding  
  - Storey range converted to midpoint  
  - Remaining lease converted to numeric years  

## Notes

- `block_avg_price` is currently set to 0 for input as a placeholder.  
- Ensure **storey range** format is correct (e.g., `10 TO 12`) for accurate prediction.  
- The app predicts resale prices based on historical HDB data from 1990 onwards.  
- This project is intended for educational and personal use.

## Author

**Chenna Pavani**  
Email: cpavani6146@gmail.com  
GitHub: [https://github.com/pavani-chenna](https://github.com/pavani-chenna/HDB-Resale-Price-Prediction-System/blob/main/Pavani_Capestone.ipynb)





