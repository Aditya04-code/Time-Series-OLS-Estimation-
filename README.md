# Time Series OLS Estimation

## Project Overview  
This project is an in-depth econometric study that replicates the findings of the research paper **"Does the Stock Market Predict Real Activity? Time Series Evidence from the G-7 Countries."** The study aims to analyze the relationship between **Industrial Production (IP)** and **stock returns** by employing several econometric models and techniques.

The project examines the relationship between industrial production and stock market activity across the **G-7 countries** using time series data. Our goal was to replicate the findings of the original research by conducting rigorous analysis with **OLS Estimation**, **Error Correction Models (ECM)**, and **ARIMA** & **GARCH** models.

## Dataset Description  
The dataset used in this analysis consists of **monthly observations** of the following indices:

- **Stock Index**: Represents the stock market for each country (nominal values).
  - **Canada**: S&P/TSX
  - **USA**: NASDAQ
  - **UK**: FTSE 100
  - **Japan**: Nikkei 225
  - **Italy**: Italian FTSE
  - **France**: CAC 40
  - **Germany**: DAX

- **Industrial Production Index (IP)**: Reflects the production output in each of the G-7 countries.

- **Consumer Price Index (CPI)**: Represents inflationary measures across countries.

The stock index data was sourced from **Refinitiv** and **TradingView**, while the **Industrial Production Index** and **Consumer Price Index** were obtained from the **International Monetary Fund (IMF)**'s **International Financial Statistics**.

The time period for the data spans several years, with **monthly observations**, and the data was transformed into **quarterly** and **annual** observations as needed for the various models.

## Objective  
The primary goal of this project is to replicate the research paper's findings by exploring the relationship between stock market returns and industrial production. Specifically, the analysis focuses on:

- Conducting **time series econometric analysis** to explore the predictive relationship.
- Utilizing **OLS (Ordinary Least Squares) estimation**, **Error Correction Models (ECM)**, and **ARIMA** and **GARCH** models to model and forecast economic activity.
- Adjusting the **Stock Index for inflation** by calculating the **Real Stock Index**, which is the **Nominal Stock Index divided by the Consumer Price Index**.

## Methodology  
1. **Data Preprocessing**:
   - Data is collected from multiple sources and cleaned for missing values.
   - The Nominal Stock Index is adjusted for inflation by dividing it by the Consumer Price Index to obtain the Real Stock Index.
   
2. **Modeling**:
   - **OLS Estimation**: Linear regression models are used to estimate the relationship between stock returns and industrial production.
   - **Lagged ECM (Error Correction Model)**: Analyzing short-term and long-term relationships between stock returns and industrial production.
   - **ARIMA**: A time series model to predict future values of industrial production and stock returns.
   - **GARCH**: Used to model volatility in stock returns and analyze market risk.

3. **Model Evaluation**:
   - Each model is evaluated using **R-squared**, **RMSE**, **MAE**, and other relevant econometric metrics to assess the model’s fit and predictive accuracy.

## Key Results  
The project reveals important insights into the relationship between **Industrial Production** and **Stock Returns** across G-7 countries. The analysis of the models shows varying degrees of predictive power, with ARIMA and GARCH models performing well in forecasting stock returns, while OLS and ECM provide robust estimates of long-term relationships.

## Data and Sources  
- **Stock Index Data**:  
  - **Canada**: S&P/TSX  
  - **USA**: NASDAQ  
  - **UK**: FTSE 100  
  - **Japan**: Nikkei 225  
  - **Italy**: Italian FTSE  
  - **France**: CAC 40  
  - **Germany**: DAX  
  
  Data sourced from **Refinitiv** and **TradingView**.

- **Industrial Production Index**: Sourced from the **IMF**'s **International Financial Statistics**.

- **Consumer Price Index**: Sourced from the **IMF**'s **International Financial Statistics**.

## Conclusion  
This project successfully replicates the original research findings and provides insights into the predictive relationship between industrial production and stock market performance in the G-7 countries. The analysis reveals how inflation-adjusted stock indices better reflect the underlying economic activity, providing more accurate predictions for economic forecasting.

## Future Work  
- Incorporate additional time series models and test other macroeconomic variables for prediction.
- Explore alternative methodologies such as **Cointegration Analysis** or **Vector Autoregression (VAR)** to assess the relationships more rigorously.
- Expand the analysis to include emerging market economies to broaden the scope of the study.

## How to Run  
1. Clone the repository:
   ```bash
   git clone https://github.com/Aditya04-code/time-series-ols-estimation.git
