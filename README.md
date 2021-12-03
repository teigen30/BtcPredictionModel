# BtcPredictionModel

Overview
This project uses the last six years of daily data for bitcoin. The data includes records for the high, low, open, close, adjusted close, and volume. A very simple model, an ARIMA model, and a Long Short-Term Memory neural network were used to attempt to create short term predictions. A model like this would helpful for people who are interested in investing in cryptocurrency but worry about the extreme volatility that comes with it. 

Business and Data Understanding
Cryptocurrencies, when looking at long term historical data, seem to be profitable in most cases. For example, a $10,000 investment into Ethereum on January 1 of 2021 would currently (12/02/2021) be worth over $57,000. However, hindsight is 20/20, and as soon as your money is invested and the price fluctuates by more than 20%, investors tend to panic, either selling due to worry that a positive spike will diminish in the near future, or that a negative spike will continue to accelerate. Providing investors with a rough prediction for short term cryptocurrency prices or percent change would help them to make more informed decisions regarding their money before they do anything in haste.

Stakeholder Audience
The stakeholder for this proposal would be the common everyday investor. As the model does not work extremely accurately, it could be made for use by others for free to either use or build on. 

Modeling
ARIMA
Initial Exploration:

Baseline Model:
The baseline model was a simple ARIMA model. It was found using the pmd arima function(?) and had a (p, d, q)(P, D, Q, m) of (1, 0, 0)(0, 0, 0, 0). 
Final Model:
The final model was a Long Short-term memory neural network that had…

Model Results
Parameter Tuning:
Made adjustments to prevent overfitting using Early Stopping and Dropout. 

Recommendations:
Our recommendation is for everyday cryptocurrency investors to use our model as a baseline model and work from there. Whether that means actually coding to enhance the model or using the model in addition to other things to help make decisions when investing.
