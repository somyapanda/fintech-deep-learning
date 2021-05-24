# fintech-deep-learning-homework

This repository contains the Jupyter notebook, accompanied with the deep learning  model as part of the Fintech homework assignment Unit14- LSTM Stock Predictor.


In this homework, we are helping investors in predicting Bitcoin price using deep learning models. These models are trained using both the FNG values and simple closing prices of the cryptocurrency. The purpose of this exercise is to evaluate the deep learning models and determine if the FNG indicator provides a better signal for cryptocurrencies than the normal closing price data.


## Files

### [LSTM Stock Predictor Closing](lstm_stock_predictor_closing.ipynb)

In this notebook, we build and trained a custom LSTM RNN that uses a 10 day window of Bitcoin closing prices to predict the 11th day closing price. These are the following tasks:

1. Prepare the data for training and testing

In this section, we have prepared the training and testing data for the model by using a rolling 10 day window to predict the 11th day closing price.

    - use the window_data function to generate the feature and target values for the model.
    - split the data into 70% training and 30% testing
    - apply the MinMaxScaler to the feature and target values
    - reshape the feature data for the model

2. Build and train a custom LSTM RNN

In this section, we have designed a custom LSTM RNN and fit (train) it using the training data.

    - define the model architecture
    - compile the model
    - fit the model to the training data


3. Evaluate the performance of the model

In this section, we evaluated the model using the test data.

    - evaluate the model using test data.
    - use the feature test data to make predictions
    - create a DataFrame of Real vs predicted values.
    - plot the Real vs predicted values as a line chart


### [LSTM Stock Predictor FNG](lstm_stock_predictor_fng.ipynb)

In this notebook, we build and train a custom LSTM RNN that uses a 10 day window of Bitcoin fear and greed index values to predict the 11th day closing price. These are the following tasks:

1. Prepare the data for training and testing
2. Build and train a custom LSTM RNN
3. Evaluate the performance of the model


## Conclusion:

From the above evaluation, we conclude that:

**Which model has a lower loss?**

The LSTM RNN model using the closing prices has a lower loss. It has a loss of 0.0203.

**Which model tracks the actual values better over time?**

The model with better results over time is the closing prices predictor.

**Which window size works best for the model?**

The window size that works better is 10.

