# Walmart Time Series Demand Prediction Analysis

## Project Overview
This project focuses on understanding and modeling product demand at Walmart using a dataset containing one year of customer transactions. The aim is to develop a predictive model for actual product demand by analyzing factors such as pricing, inventory levels, and customer demographics. Insights from this study can help Walmart optimize inventory management, improve demand forecasts, and enhance business efficiency.

---

## Features of the Project
- **Data Aggregation**:
  - Consolidated transaction-level data into a product-category-period dataset.
  - Key metrics include total quantity sold, average unit price, inventory statistics, and computed features.
- **Feature Engineering**:
  - Introduced lag variables to capture historical trends.
  - Created additional features for enhanced forecasting accuracy.
- **Modeling**:
  - Tested multiple models: Linear Regression, Random Forest, and ARIMA.
  - Implemented time-series cross-validation for proper temporal dependency handling.
- **Data Visualization**:
  - Used histograms, scatter plots, and time-series plots to explore data distributions and trends.
  - Visualized relationships between variables like price, demand, and customer loyalty.

---

## Dataset Description
### Data Source
- **Source**: Kaggle
- **File**: `walmart.csv`
- **Timeframe**: One year of customer transactions.

### Key Variables
- **Transaction Details**: Quantity sold, unit price, inventory levels.
- **Customer Attributes**: Age, income, loyalty level.
- **Environmental Factors**: Promotions, holidays, weather conditions.
- **Time-Series Information**: Period, weekday, and lagged demand.

---

## Methodology
1. **Data Aggregation**:
   - Consolidated raw transaction data by product category and period.
   - Generated summary metrics to simplify analysis.
2. **Exploratory Data Analysis (EDA)**:
   - Identified trends in sales over time.
   - Visualized distributions and correlations between key variables.
3. **Feature Engineering**:
   - Created lagged demand features for time-series forecasting.
   - Engineered variables like customer loyalty and promotions for better predictive performance.
4. **Model Development**:
   - Linear Regression: Simple baseline model.
   - Random Forest: Captured non-linear relationships and feature importance.
   - ARIMA: Specialized in time-series forecasting.
5. **Model Evaluation**:
   - Assessed using RMSE (Root Mean Squared Error).
   - Conducted time-series cross-validation to ensure temporal consistency.

---

## Key Results
- **Best Model**: Random Forest with the lowest RMSE.
- **Feature Importance**:
  - Quantity Sold: 51.87%
  - Inventory Level: 31.12%
- **Insights**:
  - Price and customer loyalty were less influential than initially hypothesized.
  - Demand predictions were more accurate for higher-demand products.

---

## Threats to Validity
- **Limited Timeframe**:
  - Data covers only one year, limiting the detection of seasonal patterns.
- **Out-of-Sample Variability**:
  - High variability in test RMSE suggests challenges in extrapolating results.
- **Lower-Demand Products**:
  - Predictions for low-demand products showed higher errors.

---

## Lessons Learned and Next Steps
- Focus on improving predictions for low-demand scenarios.
- Extend the dataset to capture seasonal and economic trends.
- Reassess the role of pricing and customer loyalty with additional data or advanced modeling techniques.

---

## Getting Started
### Dependencies
- **Programming Language**: Python
- **Libraries**:
  - pandas, numpy, seaborn, matplotlib, scikit-learn, statsmodels

### Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/walmart-demand-prediction.git
   ```
2. Load the `walmart.csv` dataset.
3. Run the provided scripts to preprocess data, train models, and visualize results.

---

## Contact
For questions or collaboration opportunities, please reach out to:

**Name**: Arturo Medina  
**LinkedIn**: [linkedin.com/in/arturo-medina](https://linkedin.com/in/arturo-medina)
