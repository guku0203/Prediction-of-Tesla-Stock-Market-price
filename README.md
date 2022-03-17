# Prediction-of-Tesla-Stock-Market-price using Linear Regression
## Introduction
Linear regression is utilized in business, science, and just about any other field where predictions and forecasting are relevant. It helps identify the relationships between a dependent variable and one or more independent variables. Simple linear regression is defined by using a feature to predict an outcome. That’s what we’ll be doing here.

Stock market forecasting is an attractive application of linear regression. Modern machine learning packages like scikit-learn make implementing these analyses possible in a few lines of code. Sounds like an easy way to make money, right?

## What is the Stock Market?
A stock market is a public market where you can buy and sell shares for publicly listed companies. The stocks, also known as equities, represent ownership in the company. The stock exchange is the mediator that allows the buying and selling of shares. 
![image](https://user-images.githubusercontent.com/83390750/158806088-bf98dc5f-d1f7-4546-a9be-e91be96de13f.png)

## Importance of Stock Market
-Stock markets help companies to raise capital.
-It helps generate personal wealth.
-Stock markets serve as an indicator of the state of the economy.
-It is a widely used source for people to invest money in companies with high growth potential.

## Stock Price Prediction
Stock Price Prediction using machine learning helps you discover the future value of company stock and other financial assets traded on an exchange. The entire idea of predicting stock prices is to gain significant profits. Predicting how the stock market will perform is a hard task to do. There are other factors involved in the prediction, such as physical and psychological factors, rational and irrational behavior, and so on. All these factors combine to make share prices dynamic and volatile. This makes it very difficult to predict stock prices with high accuracy. 

## Understanding Long Short Term Memory Network
Here, you will use a Long Short Term Memory Network (LSTM) for building your model to predict the stock prices of Google.

LTSMs are a type of Recurrent Neural Network for learning long-term dependencies. It is commonly used for processing and predicting time-series data. 
![image](https://user-images.githubusercontent.com/83390750/158806811-2ff6c864-cffc-4135-a9b9-e9ac20a7aafc.png)


From the image on the top, you can see LSTMs have a chain-like structure. General RNNs have a single neural network layer. LSTMs, on the other hand, have four interacting layers communicating extraordinarily.

LSTMs work in a three-step process.


-The first step in LSTM is to decide which information to be omitted from the cell in that particular time step. It is decided with the help of a sigmoid function. It looks at the previous state (ht-1) and the current input xt and computes the function.


-There are two functions in the second layer. The first is the sigmoid function, and the second is the tanh function. The sigmoid function decides which values to let through (0 or 1). The tanh function gives the weightage to the values passed, deciding their level of importance from -1 to 1.


-The third step is to decide what will be the final output. First, you need to run a sigmoid layer which determines what parts of the cell state make it to the output. Then, you must put the cell state through the tanh function to push the values between -1 and 1 and multiply it by the output of the sigmoid gate.

With this basic understanding of LSTM, you can dive into the hands-on demonstration part of this tutorial regarding stock price prediction using machine learning.
