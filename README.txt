AdEase Time Series

Ad Ease is an ads and marketing based company helping businesses elicit maximum clicks @ minimum cost. AdEase is an ad infrastructure to help businesses promote themselves easily, effectively, and economically. The interplay of 3 AI modules - Design, Dispense, and Decipher, come together to make it this an end-to-end 3 step process digital advertising solution for all.

You are working in the Data Science team of Ad ease trying to understand the per page view report for different wikipedia pages for 550 days, and forecasting the number of views so that you can predict and optimize the ad placement for your clients. You are provided with the data of 145k wikipedia pages and daily view count for each of them. Your clients belong to different regions and need data on how their ads will perform on pages in different languages.

This project aimed to analyze and forecast Wikipedia page views for optimizing ad placements. The following steps were undertaken:

    Data Import and Exploration:
        Imported the datasets, including daily view counts and exogenous campaign data.
        Conducted exploratory data analysis (EDA) to understand the dataset structure, check for null values, and visualize page view trends.

    Data Preparation:
        Split the page name into relevant components (Title, Language, Access Type, Access Origin) for better analysis.
        Reshaped the dataset using the melt function for a time series format, enabling easier manipulation and modeling.

    Data Visualization:
        Created bar plots to identify the top Wikipedia pages by total and mean views.
        Visualized page views over time to observe trends and patterns.

    Stationarity Testing:
        Applied the Augmented Dickey-Fuller test to assess the stationarity of the time series data, confirming that the series was not stationary.
        Utilized decomposition and differencing methods to make the series stationary.

    Modeling:
        Developed and trained a SARIMAX model, incorporating seasonal components and exogenous variables.
        Forecasted page views for the test set and evaluated the model's performance using metrics such as Mean Absolute Error (MAE) and Mean Absolute Percentage Error (MAPE).
        Implemented Facebook Prophet for forecasting, including the use of external regressors to enhance prediction accuracy.

    Forecast Evaluation:
        Compared the forecasts from both SARIMAX and Prophet models, calculating performance metrics to assess accuracy.
        Visualized the forecast results, providing insights into the expected page view trends.
