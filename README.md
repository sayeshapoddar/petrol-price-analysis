

 fuel Price Analysis Across Indian States (2017–2022)

This project explores how petrol prices changed across 15 major Indian states from 2017 to 2022 using public monthly data. The goal was to understand long-run differences between states, identify volatility, and create simple forecasts for 2023.


Dataset

* Source: Kaggle: Top 15 Indian States Petrol Prices (2017–2022)
* Frequency: Monthly
* States included: Delhi, Maharashtra, Tamil Nadu, Karnataka, Kerala, Rajasthan, Punjab, Haryana, Telangana, Assam, Gujarat, West Bengal, Bihar, Uttar Pradesh, Madhya Pradesh
* Range: May 2017 to December 2022

**Methodology**

1. Data Cleaning and Preparation

* Converted date strings (e.g., `2017_Aug`) into datetime objects
* Reshaped the dataset into long and wide
* Interpolated missing values within each state series

2. Forecasting
* Naive model (repeat last observed value)
* Rolling averages (3-month and 6-month means)
* Holt’s Linear Trend

The final output generates a 12-month forecast for 2023 for all states and visualizes predictions for selected ones.

3. **Key Findings**

Long-run pricing
* Madhya Pradesh, Telangana, and Rajasthan show the highest average petrol prices across the 6-year period.
* These differences remain over time, reflecting VAT, transport costs, and refinery cost or acess.

Volatility
* Rajasthan, Telangana, and Madhya Pradesh exhibit the largest volatility.
* States like Delhi and Gujarat remain relatively stable.

COVID-19 structural break
* All states show a noticeable upward shift after 2020, aligning with global prices and increased supply-chain costs post covid

Forecasts for 2023
* Holt’s trend forecasts project moderate increases or stabilization depending on the state’s recent trajectory.
* High-price states are expected to remain high, indicating strong long-run factors rather than temporary shocks.


Tools and Libraries

* Python
* pandas, numpy
* matplotlib, seaborn
* statsmodels 
