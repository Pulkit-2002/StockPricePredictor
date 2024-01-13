# StockPricePredictor <br>

In this project, I aim to develop a comprehensive machine learning solution for predicting stock prices, leveraging neural network models. The primary objective is to provide users with a versatile tool that can analyze historical stock data, make predictions, and aid in enhancing trading strategies. The project encompasses key stages such as data acquisition, preprocessing, model training, backtesting, and generating stock price predictions. By sharing this project on GitHub, I aim to contribute to the open-source community and provide a platform for collaborative improvement and innovation in the field of financial prediction models. <br> 

## Overview <br>

The general process for this project involves: <br>

1.Collecting stock price data to serve as features for the model. <br>
2.Preprocessing the data to create training and testing datasets. <br>
3.Utilizing a neural network to learn from the training data. <br>
4.Conducting a backtest of the model over a specified date range. <br>
5.Generating valuable predictions for stock prices. <br>
6.Enhancing trading strategies by incorporating these predictions. <br>

To clone and download the project <br>
> pip install -r requirements.txt <br>
> python LTSMModelling.py <br>

## Motivation: <br>

The motivation behind undertaking this project stems from the increasing importance of data-driven decision-making in the financial domain. Predicting stock prices accurately can significantly impact trading strategies, investment decisions, and risk management. By developing and sharing this project, I aspire to empower individuals interested in finance and machine learning to explore, understand, and contribute to the development of robust predictive models. Additionally, the project serves as a practical application of neural networks in the financial sector, fostering learning and innovation within the intersection of data science and finance. Through collaboration on GitHub, I hope to receive valuable feedback, improvements, and insights from the broader community, creating a dynamic and evolving resource for financial forecasting. <br>

## Data Aquisition <br>

To download stock price data , download stock data directly from Kaggle datasets or from Yahoo. <br>

## Data Processing (Preprocessing)

> Processing.get_train(seq_len)

## Neural Network Models

I have used 2 types of modelling in myproject i.e. Multilayer Perceptron and LTSM Modelling in order to get aquainted with Machine Learning and Neural Networks.

## Testing (Backtesting)

> back_test(strategy, seq_len, ticker, start date, end_date, dim)

## Predictions

> data = pdr.get_data_yahoo("AAPL", "2024-10-09", "2023-07-28")
> stock = data["Adj Close"]
> X_predict = np.array(stock).reshape((1, 10)) / 200
> print(model.predict(X_predict)*200)
