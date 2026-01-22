# Final-Analysis-Project
In this project I have used a Linear Regression Model as well as the ARIMA and ARIMAX model to make predictions on and predict the trend of future values of the currency pair EUR/USD.

The first part prediction model used is Linear Regression.The application of a linear Regression Model might seem counterintuative at first but as can be observed the model works well in predicting future values of the mid price of the currency pair.It works the same as any Linear Regression model the only difference is that the tarhet variable Y will be advanced in time.This equation describes it better:

                                          X ( t ) =X[x1(t),x2(t),x3(t),...,xn(t)] , y(t+n)

The second model I used is the ARIMA model. The ARIMA model incorporates the autoregressive model, as well as a differencing order and a moving average. In our model, since we will train over a shorter range, our data will be stationary, thus eliminating the need for differencing.
The moving average calculates an error term from the training data, where the error term is determined using the following formula.

                                                             E(t)=X(t)-Xest(t)
The output at time X(t)will be calculated as a linear combination of past errors computed at different times, depending on the order q

                                                    X(t) = C + 1X(t-1)+.......qX(t-q) 

The last model I used is the ARIMAX model.An ARIMAX model is an extension of the ARIMA model in which additional variables are used to improve prediction. When predicting using exogenous variables, we assume that we have access to both past and future values of these variables. Therefore, it is important to choose a variable that is practically obtainable.Analyzing the statistical properties of each variable, the variable we have chosen is Bid Close (BC). Its values are dispersed and can be predicted from their past values. The high standard deviation means that it will provide us with more information.
