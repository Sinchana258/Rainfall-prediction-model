#  Rainfall Prediction using Machine Learning  

##  Project Overview  
This project predicts **daily and annual rainfall** for Udupi district using **historical NASA POWER weather data (1990–2024)**.  
We implemented **Random Forest** and **Gradient Boosting** models to capture rainfall patterns and trends.  

The system helps in **agriculture planning, water resource management, and climate studies** by providing accurate rainfall forecasts.  

---

##  Features  
-  **Data Preprocessing** → Handles missing values & outliers using IQR and capping  
-  **Feature Engineering** → Extracts seasonal & climatic features (temperature, humidity, soil wetness, wind, etc.)  
-  **Random Forest** → Handles non-linear weather relationships  
-  **Gradient Boosting** → Improves prediction accuracy through boosting  
-  **Evaluation Metrics** → RMSE & R² Score  
-  **Daily & Annual Predictions** → Can predict rainfall for any given date or year  

---

## 📂 Dataset  
- **Source:** [NASA POWER](https://power.larc.nasa.gov/data-access-viewer/)  
- **Location:** Udupi District, India (Lat: 9.1644, Lon: 76.7423)  
- **Period:** 1990 – 2024  
- **Target Variable:** `PRECTOTCORR` (Corrected Daily Precipitation in mm/day)  

---

##  Tech Stack  
- **Language:** Python  
- **Libraries:**  
  - `pandas`, `numpy` → Data handling  
  - `matplotlib`, `seaborn` → Visualization  
  - `scikit-learn` → Machine Learning models  

---

##  Model Performance  

| Model             | Train R² | Test R² | Train RMSE | Test RMSE |
|-------------------|----------|---------|------------|-----------|
| Random Forest     | 0.97     | 0.76    | 86.69      | 159.60    |
| Gradient Boosting | 0.999    | 0.74    | 0.636      | 166.51    |

✅ Gradient Boosting performed best overall, especially for capturing monsoon trends.  

---
