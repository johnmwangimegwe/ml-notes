# Machine Learning Notes 25 a - Zindua School
Access the notes your technical mentors used to teach your live classes in your machine learning modules. 
The folders are based on your class, but you are free to explore notes from previous classes (and other technical mentors) to enrich your knowledge. In every class folder, notes will be structured as follows:
1. Notebooks covering the weekly content usually named as : `week-##-...`
2. Any data files used in the weekly content, usually available in a data subfolder
3. Additionally, the `kaggle-guide` folder (separate from the class notes) contains a general guide for working on Kaggle projects

In this class 25a - We will be using the following projects in class : 
1. Data Cleaning - Bengaluru Housing Problem
2. Carlifornia housing problem - Regression 
3. Classification - Telkom Churn Analysis
4. Model Evaluation and Error Analysis - Boston House Problem


For your projects, ensure you have a well written Readme document. The following are critical areas the Readme has to touch on : 
| Section | Example | 
|--------|--------| 
| **1. Project Goal**| Forecast the hourly total load (demand)  for one year, and possibly the renewable electricity production (from solar and wind) also, based on weather data and three previous years of hourly generation data for all of Spain | 
|**2. Context/ Problem Statement **| Accurate power generation forecasts, both short term and long term, are critical to a green energy future. Accurate forecasts enable renewable generators to correctly price their energy and maximize contribution from renewable sources (while minimizing carbon sources), and are important to operators for system stability and planning | 
|**3. Criteria for Success / Performance Measurement** | This model will be successful if the forecasted total load, are close (within approximately 10%) to the actual values | 
| **4. Scope of Solution Space / Model to be Used and Data Transformations Required** | Electricity demand forecasting is often done using time series forecasting when dealing with data containing only time and demand variables. Electricity demand is strongly dependent on exogenous variables like temperature, humidity, etc. Thus, with weather data available, regression may also be a relevant model choice. Our scope will involve testing and comparing several types of models potentially including, but not limited to:  ARIMA, SARIMAX, XGBoost | 
|**5. Constraints / Potential Challenges** | Three years of training data may not be enough to accurately predict the targets, especially if one year was anomalous with regards to weather or demand.| 
| **6. Stakeholders** | The stakeholders for such a real world project would be the system operator, and wind and solar generators. | 
| **7. Key Data Sources** | The weather data that will be included in the model includes hourly: time, temperature, pressure, humidity, wind speed/direction, and weather descriptor (clouds, few clouds, clear, etc…). The hourly energy production data includes time, generation by method (approximately 21 different methods), day ahead solar generation forecast, day ahead wind generation forecast, total load forecast, total load actual, day ahead price per MWH, and actual price per MWH. All data is sourced from a [Kaggle](https://www.kaggle.com/datasets/nicholasjhana/energy-consumption-generation-prices-and-weather) dataset that was sourced from [Open Weather](https://openweathermap.org/api), [ENTSOE](https://transparency.entsoe.eu/dashboard/show) transparency platform, and [Red Electrica](https://www.esios.ree.es/en/market-and-prices).| 
