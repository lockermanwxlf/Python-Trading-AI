# Price Action

The idea behind this is to use the delta between today's close and n day back's close to predict 5 day's from now close.

I would like to change this to LSTM so there's a bit of prior context in the input data rather than it just being a formula.

The actual price delta prediction is not helpful, but using >0 = buy and <=0 = no buy leads to more profit than what buy and hold SPY itself gives on average.

It was trained from 2022-2024, which includes both a bullish and bearish trend. Additionally, each time it was trained it would either
yield returns much better than buy and hold or returns slightly worse than buy and hold. I would like to split the dataset into bearish 
and bullish datasets to see if that classification leads to more consistent profit.
