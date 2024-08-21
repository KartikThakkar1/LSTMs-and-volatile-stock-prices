# Stacked LSTMS to forecast the opening price of the AMZN stock.
  

* ### The stock price data was pulled through the [tiingo API](https://www.tiingo.com/) in a dataframe format using the [pandas-datareader](https://pandas-datareader.readthedocs.io/en/latest/) module.
* ### A time step of 100 was used for training.

* ### It must be noted that in this particular data, there is a sudden drop in the opening price of the stock as seen in the plot below.
![data_trend](https://github.com/user-attachments/assets/aea45266-4d8b-4eca-a37a-5a4915867219)

* ### Since this is time series data, the train and test split had to be done keeping that in account. Moreover, the train test split was 70-30. Additionally, most of the data in the train set had a very high value compared to the test set's values. In my opinion, this is what affected the training performance.
  

| Dataset     | Size          | RMSE Value  |
| ------------- |:-------------:| -----:|
| Train     | 879 | 125.54 |
| Test      | 378     |  7.67 |


![traintesttrends](https://github.com/user-attachments/assets/ae2d3c2f-5b16-4559-89fd-d3c7f1435b41)

* ### Predictions
  ![preds](https://github.com/user-attachments/assets/c32f2596-bcb0-442e-aed2-a52bcca8791d)

* ### Forecast for the open price for next 30 days :
  ![fcast](https://github.com/user-attachments/assets/e9817412-0e87-41fe-ac70-1f8223476ba0)

  ![fcast2](https://github.com/user-attachments/assets/0b6ea473-819c-4600-b000-47cadcca85f9)






