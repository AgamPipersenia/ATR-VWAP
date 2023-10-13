# ATR-VWAP
In the code, We first downloaded the data using yfinance for 2 years timeframe, with 1 hour interval. Then we calculated the average true range of the stock. To do so, we first calculated the true range, which was maximum of high-low, mod(high-prevclose) low and mod(low-prev close). Then atr was moving average of true range over 14 day interval. Then we calculated the Vwap values of the stock, using typical price.

Then, in order to combine the vwap values and atr, we generated buy/sell signals, which covered both the indicators. The atr was used to find if the typical price of a stock was less than lower or greater than upper band of the atr. And the vwap value we used to determine if the closing price was above or below the vwap value, thereby buying or selling the stock respectively.

Due to lack of time, we could’nt analyze the choice of stock for these indicators. However, upon backtesting on 15-20 stocks, we chose our stocks to be ITC,NTPC,ADANIENT,TITAN,CIPLA. And the investment in all of these stocks were 40%,30%,10%,10%,10%, solely based on the returns so obtained. Due to lack of time, we could not combine the method to divide the investment in the ratio we desired, so we have submitted respective code for each of the stock, and in a new file calculate total returns.

Contributors- Agam Pipersenia and Naman Sethi
