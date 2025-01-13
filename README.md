## Project Description

This project focuses on predicting the severity of accidents using the **US Road Accidents dataset**. By analyzing accident-related data, including factors such as weather conditions, road types, time of day, and more, we aim to develop a machine learning model that can predict the severity of road accidents.

### Key Objectives:
1. **Data Cleaning & Preprocessing**:
   - Dropped unnecessary columns.
   - Handle missing values in categorical and numerical columns.
   - Optimize the memory usage of the dataset.
   - Remove irrelevant and highly correlated features.
   - Detect and remove outliers using the IQR method.
   - Create new features, such as accident duration, time-based features, and others, to improve model performance.

### Model Selection and Ensemble

1. **Individual Models**: The following machine learning models were trained on the training set:
   - **XGBoost (XGB)**: A gradient boosting model known for its high performance and speed.
   - **LightGBM (LGBM)**: A fast and efficient gradient boosting framework that is optimized for large datasets.
   - **CatBoost**: A gradient boosting model that handles categorical features automatically and performs well with less hyperparameter tuning.

2. **Ensemble Method**: The predictions from the individual models (XGB, LGBM, and CatBoost) were combined using an ensemble technique to improve the overall prediction accuracy and robustness. This allows the strengths of each model to complement each other.

3. **Final Model**: The ensemble model outperformed the individual models in terms of accuracy and robustness on the test set, providing more reliable predictions for accident severity.

### Analysis & Recommendations:
   - Identify patterns and correlations in the data that affect accident severity.
   - Provide data-driven recommendations to reduce accident risks based on weather, time of day, and other factors.

### Target Variable:
- **Accident Severity**: The severity of accidents, ranging from minor to severe(0-3) with grater the number, severe the accident.

### Instructions to run:
1. Clone the repository:
   ```bash
   git clone https://github.com/asasmit/Accident_USA
2. Install Libraries
   ```bash
   pip install -r requirements.txt
3. Download the dataset from [Link Text](https://drive.google.com/file/d/1edKrdWNOcgbAo2JtckX-PEyM0FdEq4EG/view?usp=drive_link) in the same directory.
