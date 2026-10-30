# Algerian Forest Fires - FWI Prediction

This project builds a regression machine learning model to predict the **Fire Weather Index (FWI)** based on meteorological data and forest fire indices from the Algerian Forest Fires dataset.

## Dataset
- **File:** `4-Algerian_forest_fires_dataset.csv`[cite: 3]
- **Features:** Temperature, Relative Humidity (`RH`), Wind Speed (`Ws`), Rainfall (`Rain`), Fine Fuel Moisture Code (`FFMC`), Duff Moisture Code (`DMC`), Drought Code (`DC`), Initial Spread Index (`ISI`), Build Up Index (`BUI`), Classes, and Region[cite: 3].
- **Target Variable:** `FWI` (Fire Weather Index)[cite: 3].

## Workflow & Methodology
1. **Data Cleaning & Preprocessing:** 
   - Handled missing values, removed unneeded rows/columns, and cleaned column names[cite: 3].
   - Corrected data types for numerical and categorical features[cite: 3].
   - Converted target classes into binary format (`0` for `not fire`, `1` for `fire`)[cite: 3].
2. **Exploratory Data Analysis (EDA):** 
   - Inspected statistical distributions and visualized feature correlations using heatmaps[cite: 3].
3. **Feature Selection:** 
   - Checked multicollinearity and dropped highly correlated features (threshold > 0.85) to optimize model performance[cite: 3].
4. **Train-Test Split:** 
   - Divided the dataset into training and testing sets (75% train, 25% test) using `scikit-learn`[cite: 3].
5. **Standardization:** 
   - Initialized `StandardScaler` for feature scaling and normalization[cite: 3].

## Technologies & Libraries Used
- **Python**[cite: 3]
- **Pandas & NumPy** (Data manipulation and cleaning)[cite: 3]
- **Matplotlib & Seaborn** (Data visualization and correlation heatmaps)[cite: 3]
- **Scikit-Learn** (Train-test splitting and preprocessing tools)[cite: 3]
