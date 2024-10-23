# AdEase Time Series

### Goal
The goal of this project is to analyze and forecast Wikipedia page views for 145k pages over 550 days, helping AdEase optimize ad placements for clients across different regions and languages. By forecasting page views, the project aims to predict ad performance and improve ad placement strategies for businesses.

### Project Overview
AdEase is an ads and marketing company that helps businesses achieve maximum clicks at minimum cost. AdEase provides a digital advertising solution through three AI modules: Design, Dispense, and Decipher. This project focuses on analyzing Wikipedia page views to optimize ad placement using time series forecasting techniques.

### Steps Undertaken:

#### 1. Data Import and Exploration:
- Imported the datasets, including daily view counts and exogenous campaign data.
- Conducted exploratory data analysis (EDA) to understand the dataset structure, check for null values, and visualize page view trends.

#### 2. Data Preparation:
- Split the page name into relevant components (Title, Language, Access Type, Access Origin) for better analysis.
- Reshaped the dataset using the melt function for a time series format, enabling easier manipulation and modeling.

#### 3. Data Visualization:
- Created bar plots to identify the top Wikipedia pages by total and mean views.
- Visualized page views over time to observe trends and patterns.

#### 4. Stationarity Testing:
- Applied the Augmented Dickey-Fuller test to assess the stationarity of the time series data, confirming that the series was not stationary.
- Utilized decomposition and differencing methods to make the series stationary.

#### 5. Modeling:
- Developed and trained a SARIMAX model, incorporating seasonal components and exogenous variables.
- Forecasted page views for the test set and evaluated the model's performance using metrics such as Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE).
- Implemented Facebook Prophet for forecasting, including the use of external regressors to enhance prediction accuracy.

#### 6. Forecast Evaluation:
- Compared the forecasts from both SARIMAX and Prophet models, calculating performance metrics to assess accuracy.
- Visualized the forecast results, providing insights into the expected page view trends.

