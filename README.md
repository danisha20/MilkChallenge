# Prediction of Basic Supplies

This repository uses data analytics and recurrent neural networks to predict the price of Milk in Chile. 

**Required Packages**

    Python 3.8.5
    tensorflow==2.3.0
    keras == 2.4.3
    sklearn==0.20.2
    numpy==1.19.1
    pandas==1.1.1
    matplotlib== 3.2.2
    seaborn == 0.11.0
    scipy == 1.5.2

**Datasets**

The datasets used are the following : 

- precipitaciones.csv 
- banco_central.csv
- precio_leche.csv 
- ipc_data.csv


**Results**

Test set Results: 

- MAE: 11.2841
- RMSE: 14.77
- AIC:  316.34

![alt text](https://github.com/danisha20/SpikeChallenge/blob/main/lossfunc_epochs.png)

![alt text](https://github.com/danisha20/SpikeChallenge/blob/main/forecast.png)

** Conclusions**

During the analysis of this project, we observed that the milk's price in Chile experiences high volatility. In our approach to predict this variable, we identified several covariates that presented periodic fluctuation and trends and had to be converted into a stationary process to feed it to the time-series model. We performed additional preprocessing steps, such as winsorization of the extreme values, duplicate removal,  missing value imputation, and a differencing transformation. We also performed feature engineering by including additional variables to our dataset and transforming some of the variables to structure the data as a supervised learning problem. Finally, we build a model to predict the price of the latest data available using an LSTM model. The model results have a MAE of 11.28, which might be improved by performing tunning, exploring other preprocessing techniques, as well as including other variables that can deliver more information. 


**Next Steps**

- Fine Tune model hyperparameters 
- Evaluation with additional features
- Exploring dimensional reduction techniques
- Smoothing the data 
- Comparing with traditional time series methods. 

**References**

- Mosheim, R. (2012). A Quarterly Econometric Model for Short-Term Forecasting of the US Dairy Industry (No. 1488-2016-123440).

- https://www.ine.cl/estadisticas/economia/indices-de-precio-e-inflacion/indice-de-precios-al-consumidor

- https://machinelearningmastery.com/convert-time-series-supervised-learning-problem-python/
