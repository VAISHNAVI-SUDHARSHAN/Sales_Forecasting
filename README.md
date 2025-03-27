# Sales Forecasting with Machine Learning

## Project Overview
This repository contains a project completed as part of a Data Science Internship Assignment at Wiseanalytics. The project involves building a machine learning model to predict future sales for various product families across different stores in Ecuador. The sales predictions are influenced by external factors such as promotions, holidays, oil prices, and economic conditions. The goal is to understand how these factors impact sales and develop an accurate forecasting model.

The project is divided into two parts:

**Part 1**: Data Processing and Feature Engineering

**Part 2**: Model Selection, Forecasting, and Evaluation

## Dataset

The dataset consists of the following files:

- **train.csv**: Historical sales data.
- **test.csv**: Test set for which sales need to be predicted.
- **stores.csv**: Metadata about store locations and clusters.
- **oil.csv**: Daily oil prices, which impact the Ecuadorian economy.
- **holidays_events.csv**: Information about holidays and special events.

## Project Workflow

### Part 1: Data Processing and Feature Engineering 
1. **Data Cleaning**:
   - Handle missing values in oil prices using interpolation.
   - Convert date columns into proper datetime formats.
   - Merge data from multiple sources (stores, oil, holidays).

2. **Feature Engineering**:
   - **Time-based Features**: Extract day, week, month, year, day of the week, and seasonal trends.
   - **Event-based Features**: Create binary flags for holidays, promotions, and special economic events.
   - **Rolling Statistics**: Compute moving averages and rolling standard deviations.
   - **Store-Specific Aggregations**: Aggregate sales based on store type and product family.

3. **Exploratory Data Analysis (EDA)**:
   The project includes an exploratory data analysis (EDA) phase to visualize key trends in the dataset, including:

- **Sales over Time**: Analyzing overall sales trends.
- **Sales Before/After Holidays**: Understanding sales fluctuations during holidays.
- **Oil Price vs Sales**: Analyzing the relationship between oil prices and sales.

4. **Documentation**:
   - Document the preprocessing steps in the Jupyter Notebook with clear explanations of each feature and its role in forecasting.

### Part 2: Model Selection, Forecasting, and Evaluation 

1. **Model Training**:
   - Train the following forecasting models:
     - **Naïve Forecasting**: Baseline model assuming future sales = previous sales.
     - **ARIMA**: A traditional time series model.
     - **Random Forest Regressor**: Tree-based model to capture non-linear relationships.
     - **XGBoost**: Gradient boosting model for improved accuracy.
     - **LSTM (Long Short-Term Memory)**: Deep learning model for time series forecasting.
   - **Bonus**: Optional Prophet model for handling seasonality.

2. **Model Evaluation**:
   - Evaluate models using performance metrics such as **RMSE**, **MAPE**, **R² Score**, and visual inspection of predicted vs. actual sales.

3. **Visualization**:
   - Plot historical sales data and predicted sales for each model.
   - Visualize model performance comparisons using error metrics.
   - Display feature importance for models like Random Forest/XGBoost.

4. **Business Insights**:
   - Summarize which model performed best and explain why.
   - Discuss the influence of external factors like holidays, oil prices, and promotions on model predictions.
   - Provide business strategies to improve sales forecasting, such as inventory planning and targeted promotions.

## Technologies Used

- **Python**: Primary programming language for data processing and modeling.
- **Pandas**, **NumPy**: Data manipulation and analysis.
- **Scikit-learn**: Machine learning models and tools.
- **XGBoost**, **LightGBM**: Gradient boosting models.
- **Keras/TensorFlow**: For training LSTM models.
- **Statsmodels**: For ARIMA modeling.
- **Matplotlib**, **Seaborn**: Data visualization.

## 📫 Contact

If you have any questions or suggestions, feel free to reach out:

- **Name:** Vaishnavi S 
- **Email:** [vaishu4502@gmail.com](mailto:vaishu4502@gmail.com)  
- **LinkedIn:** [https://www.linkedin.com/in/vaishnavisudharshan/](https://www.linkedin.com/in/vaishnavisudharshan/)  
- **GitHub:** [https://github.com/VAISHNAVI-SUDHARSHAN](https://github.com/VAISHNAVI-SUDHARSHAN)
  
## How to Run the Project

### Requirements

Install the necessary dependencies using `pip`:

```bash
pip install -r requirements.txt





