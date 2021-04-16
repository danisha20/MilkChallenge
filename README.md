# Prediction of Basic Supplies

This repository uses data analytics and recurrent neural networks to predict the price of Milk in Chile. 

** Required Packages **

    Python 3.8.5
    tensorflow==2.3.0
    keras == 2.4.3
    sklearn==0.20.2
    numpy==1.19.1
    pandas==1.1.1
    matplotlib== 3.2.2
    seaborn == 0.11.0
    scipy == 1.5.2

** Datasets **

The datasets used are the following : 

- precipitaciones.csv 
- banco_central.csv
- precio_leche.csv 
- ipc_data.csv


** Results **

Test set Results: 

- MAE: 11.2841
- RMSE: 14.77
- AIC:  316.34

![alt text](https://github.com/danisha20/SpikeChallenge/blob/main/lossfunc_epochs.png)

![alt text](https://github.com/danisha20/SpikeChallenge/blob/main/forecast.png)

** Next Steps **

- Fine Tune model hyperparameters 
- Evaluation with additional features
- Exploring dimensional redction techniques
- Smoothing the data 
- Comparing with traditional time series methods. 

** References **

- Mosheim, R. (2012). A Quarterly Econometric Model for Short-Term Forecasting of the US Dairy Industry (No. 1488-2016-123440).

- https://www.ine.cl/estadisticas/economia/indices-de-precio-e-inflacion/indice-de-precios-al-consumidor

- https://machinelearningmastery.com/convert-time-series-supervised-learning-problem-python/
