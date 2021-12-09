# BtcPredictionModel

## Overview

This project uses the last six years of daily data for bitcoin. The data includes records for the high, low, open, close, adjusted close, and volume. A very simple model, an ARIMA model, and a Long Short-Term Memory neural network were used to attempt to create short term predictions. A model like this would be helpful for people who are interested in investing in cryptocurrency but worry about the extreme volatility that comes with it.

### Business and Data Understanding
Cryptocurrencies, when looking at long term historical data, seem to be profitable in most cases. For example, a $10,000 investment into Ethereum on January 1 of 2021 would currently (12/02/2021) be worth over $57,000. However, hindsight is 20/20, and as soon as your money is invested and the price fluctuates by more than 20%, investors tend to panic, either selling due to worry that a positive spike will diminish in the near future, or that a negative spike will continue to accelerate. Providing investors with a rough prediction for short term cryptocurrency prices or percent change would help them to make more informed decisions regarding their money before they do anything in haste.

### Stakeholder Audience
The stakeholder for this proposal would be the common investor. As the model does not work extremely accurately, it could be made for use by others for free to either use or build on. 

## Modeling

ARIMA:

An ARIMA model was created by hand and then also using auto ARIMA using the percent change data. The best model was the (1, 0, 0)(0, 0, 0, 0) intercept model. Predictions for the models were less than impressive, with none of the 17 day forecast indicating a negative change in price

Baseline Model:

The baseline model was a simple ARIMA model. It was found using the pmd arima function and had a (p, d, q)(P, D, Q, m) of (1, 0, 0)(0, 0, 0, 0). 
Final Model:

Neural Network:

The final model was a Long Short-term memory neural network that had an LSTM layer and a Dense (16) layer. It used 4 neurons with a batch size of 10. The model was not accurate in predicting th eprice of bitcoin, and had a 40% accuracy rate in determining whether the price would increase or decrease.


Recommendations:

Our recommendation is for everyday cryptocurrency investors to use our model as a baseline model and work from there. Whether that means actually coding to enhance the model or using the model in addition to other things to help make decisions when investing. The findings from this research also indicate that there will likely never be a truly accurate prediction model for cryptocurrencies or even stocks for that matter. This is because of something that we can learn from the model, that being that the price of bitcoin depends on far more than simply the recent prices and volumes.

To view my presentation, please follow this [link.](https://www.canva.com/design/DAExthpdT8w/1idvz7kjvm5h_ja11NAvMw/view?utm_content=DAExthpdT8w&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)
