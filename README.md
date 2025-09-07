# product-sales-forcast-
End-to-end product sales forecasting project using EDA, hypothesis testing, ML models, and Tableau dashboards
📊 Product Sales Forecasting
1. Problem Statement

In the competitive retail industry, the ability to predict future sales accurately is crucial for operational and strategic planning. Product sales forecasting aims to estimate the number of products a store will sell in the future, based on various influencing factors such as store type, location, regional characteristics, promotional activities, and temporal variations (holidays and seasons).

This project focuses on developing a predictive model using historical sales data from different stores to forecast future sales and support better business decision-making.

2. Need and Use of Product Sales Forecasting

Accurate sales forecasting helps retailers in multiple ways:

Inventory Management: Maintain optimal stock levels and reduce wastage.

Financial Planning: Estimate revenue and budget allocation effectively.

Marketing & Promotions: Plan campaigns and offers around sales peaks and troughs.

Supply Chain Optimization: Improve logistics, distribution, and production schedules.

Strategic Decisions: Enable market entry, store expansion, and capital expenditure planning.

3. Dataset

📂 Dataset Link

Data Description

ID: Unique identifier for each record

Store_id: Unique identifier for each store

Store_Type: Type of store (categorical)

Location_Type: Classification of store’s location (e.g., urban, suburban)

Region_Code: Geographical region code

Date: Date of record

Holiday: (1 = Yes, 0 = No)

Discount: Discount offered (Yes/No)

#Order: Number of orders on the given day

Sales: Total sales amount

4. Tableau Visualizations

Data visualization provides critical insights for stakeholders. Tableau dashboards developed:

Sales Performance Dashboard

Time series sales trends (year → month → day drilldown)

Sales distribution by store type & location

Regional Sales Analysis

Compare regions by sales, orders, and average order size

Promotional Impact Analysis

Sales with vs. without discounts

Holiday vs. non-holiday performance

Operational Insights Dashboard

Relationship between orders and sales

Stock management indicators

Forecast Evaluation Dashboard

Forecasted vs. Actual sales comparison

Error metrics (MAE, RMSE) visualization

👉 Interactive filters allow slicing data by date, region, store type, holiday, and discounts.

5. Exploratory Data Analysis (EDA) & Hypothesis Testing
EDA Steps

Univariate Analysis: Sales & order distributions (histograms, boxplots)

Bivariate Analysis: Discounts/holidays vs. sales correlations

Time Series Analysis: Seasonality, trend, cyclic behavior

Categorical Analysis: Sales by store type, location, region

Missing Value Handling: Imputation strategies

Outlier Detection: Identification & treatment

Hypothesis Testing

Discounts Impact: Sales ↑ on discount days → t-test

Holiday Effect: Sales ↑ on holidays → t-test / ANOVA

Store Type Sales: Sales vary across store types → ANOVA

Regional Variability: Sales vary by region → Kruskal-Wallis / ANOVA

Orders vs. Sales: Positive correlation → Pearson / Spearman correlation

6. Machine Learning Modeling
Data Processing

Missing value imputation

Feature engineering (time-based aggregates, ratios, interactions)

Transformation: Scaling (Standardization/Normalization), Encoding (One-Hot/Label)

Train-test split for objective evaluation

Model Selection
📈 Final Model Performance
🔹 Baseline Model: Linear Regression

MAE: 3360.82

MSE: 21,924,104.88

RMSE: 4682.32

R²: 0.94

🔹 Complex Model: Random Forest Regressor

MAE: 2036.04

MSE: 8,740,456.19

RMSE: 2950.26

R²: 0.98

✅ The Random Forest Regressor significantly outperformed the baseline linear regression model, reducing error by ~40% and achieving an R² of 0.98, meaning it explains almost all the variance in sales data.

Baseline: Linear Regression

Tree-Based Models: Random Forest, XGBoost, LightGBM

Time Series Models: ARIMA, SARIMA, Prophet

Deep Learning: LSTM for sequence forecasting

Ensemble Models: Blending and stacking

Model Evaluation

Metrics: MAE, MSE, RMSE, MAPE

Cross-validation: Time-series split CV

Residual Analysis: Ensures patterns are modeled

7. Insights & Recommendations

Discounts and holidays significantly impact sales, confirming promotional strategies are effective.

Certain store types and regions consistently outperform others → strategic expansion opportunities.

Orders strongly correlate with sales → operational efficiency plays a role.

Forecasting models enable proactive inventory and staffing decisions.
