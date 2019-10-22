# Energy-Consumption-Time-Series

***

## Individual household electric power consumption Data Set

***

#### Primarily trying to device the method that could be used to forecast energy consumption of the upcoming month, based on one months data only. A lot of experimentations done over different models. The experimentation is demonstrated and results are plotted as well.

#### **The 5 methods that are worked upon are:**

> ####   1 - ARIMA Forecasting for 1 timestep and for whole month
> ####   2 - Facebook Prophet forecasting based on variable amount of training data
> ####   3 - Using Auto Regression (AR) with walk-forward validation 
> ####   4 - Using Moving Average (MA) with anamoly detection within data
> ####   5 - Using Deep Learning for Time Series modeling


***

#### The accuracy over here does not depend on the individual daily predictions that are calculated against yhat and true value. The Goal here is to predict the overall energy consumption in the month. Therefore, the individual predictions may not seem as accurate as they should be, but the commulative monthly energy consumptions (sum of yhat) when compared against the actual monthly consumption (from the test set) could potentially have better results

***


#### The accuracy of overall energy consumption is deduced through the following simple metric:

> #### **Percent Error = ( |Experimental Value – Theoretical Value| ÷ Theoretical Value) x 100**

### NOTE
#### You will have to clean and preprocess the data that you download for missing values. For help with that preprocessing, refer to the reference 1 and 2 of **Jason Brownlee's machinelearningmastery blog.**

### Refrences
> https://machinelearningmastery.com/how-to-develop-an-autoregression-forecast-model-for-household-electricity-consumption/

> https://machinelearningmastery.com/multi-step-time-series-forecasting-with-machine-learning-models-for-household-electricity-consumption/

> https://pythondata.com/forecasting-time-series-autoregression/

> #### Dataset: https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption
