# Housing Price Prediction using Machine Learning
# 🔹Project Overview
This project focuses on building and evaluating regression models to predict **median house prices** in California districts using demographic and geographic features.

# 🔹Problem 
Predict the **median house value** of California districts based on income, population statistics, and geographic location.

# 🔹Dataset
* **Name:** California Housing Dataset
* **Source:** scikit-learn (`fetch_california_housing`)
* **Size:** 20,640 observations
* **Target Variable:** `MedHouseVal` (median house value, in units of 100,000 USD)
### Features

| Feature    | Description                  |
| ---------- | ---------------------------- |
| MedInc     | Median income in block group |
| HouseAge   | Average house age            |
| AveRooms   | Average number of rooms      |
| AveBedrms  | Average number of bedrooms   |
| Population | Block group population       |
| AveOccup   | Average number of occupants  |
| Latitude   | Latitude                     |
| Longitude  | Longitude                    |

## Project Workflow

### 1. Exploratory Data Analysis (EDA)
* Descriptive statistics
* Target distribution analysis
* Correlation heatmap to understand relationships between variables

### 2. Data Preprocessing
* Feature and target separation
* Train/Test split (80% / 20%)
* Feature scaling using `StandardScaler` (for Linear Regression)

### 3. Models Implemented
* **Linear Regression** (Baseline model)
* **Random Forest Regressor** (Non-linear model)

### 4. Evaluation Metrics
To properly evaluate regression models, the following metrics were used:
* **MAE (Mean Absolute Error)**
* **RMSE (Root Mean Squared Error)**
* **R² Score**
> Accuracy was intentionally not used, as it is not suitable for regression problems.

---

## 📈 Model Performance (Example Results)

| Model             | MAE   | RMSE  | R²     |
| ----------------- | ----- | ----- | ------ |
| Linear Regression | ~0.53 | ~0.74 | ~0.60  |
| Random Forest     | Lower | Lower | Higher |

**Random Forest** outperformed Linear Regression by capturing non-linear relationships in the data.

---

## Model Interpretation

Feature importance from the Random Forest model shows that:
* **Median income (MedInc)** is the most influential feature
* **Geographic location (Latitude & Longitude)** also plays a significant role
This aligns with real-world economic expectations.

---

## Prediction Example (Sanity Check)
A hypothetical district was created to validate model behavior.
* **Base prediction:** ~343,779 USD
* **After increasing median income:** ~478,827 USD
* **Difference:** ~135,049 USD

This sanity check confirms that the model responds logically to changes in key features.

---

## Key Skills Demonstrated
* Data exploration and visualization
* Regression modeling
* Model evaluation and comparison
* Feature importance interpretation
* Practical prediction and validation

---

## Conclusion
This project demonstrates a complete regression pipeline, from data exploration to prediction and interpretation. The Random Forest model achieved the best performance and provided interpretable results consistent with real-world expectations.

---

## Technologies Used
* Python
* pandas, numpy
* matplotlib, seaborn
* scikit-learn

---

## Author
Master’s graduate in **Data Management and Massive Data Analysis** / **gestion et analyse des donneés massives**
