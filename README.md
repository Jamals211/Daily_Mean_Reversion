# Daily_Mean_Reversion

The Daily Mean Reversion approach was formulated based on the observation that stocks tend to rise in the morning and lose momentum in the afternoon, and vice versa for a heavy decline in the morning followed by a rise. To determine if a stock experienced a major movement in the morning above a certain threshold (X bps) in either direction and a subsequent reversion in the opposite direction, a 3-minute chart for a given week can be examined. 

![image](https://user-images.githubusercontent.com/66137235/233871851-9d704a7c-fc72-46b1-a08b-ce0f45cf9f46.png)

![image](https://user-images.githubusercontent.com/66137235/233871873-b75a16f4-85bc-4f4e-8d2d-b9f917d6b421.png)

![image](https://user-images.githubusercontent.com/66137235/233872349-8dfa0d05-6c72-4810-8e91-637219d9780f.png)


The provided examples demonstrate this phenomenon, with each showing a significant movement in one direction followed by a reversion back to the mean. The Daily Mean Reversion can be a profitable trading strategy when there is a well-defined cutoff, trading timeframe, and exit strategy in place. It is important to note that the strategy encountered resistance in each example, which could explain the mean reversion. However, the Daily Mean Reversion was observed before the trend hit the resistance line, and implementing a stop loss is crucial to mitigating losses.


![image](https://user-images.githubusercontent.com/66137235/233873338-76481104-7947-4b6a-8b14-f90c4139ea1c.png)


This quantitative strategy looked at the SPY's events where there was a 0.25 bps movement in the morning in either direction, then bought a reversal trade to determine if there was a return on investment. Unfortunately, the results showed a negative return on investment when buying when the market drops and selling when it rises, likely due to the absence of a stop loss and a good reason for market movements upwards. However, the strategy did well over the last few months when the market was declining slowly, and returns were positive when the market declines and then bounces back.

![image](https://user-images.githubusercontent.com/66137235/233874291-e6c1eb27-fe62-46fe-b808-7f1366526899.png)

When only examining when the market declines, the strategy performs better, while selling expecting a decline when the market rises by 0.25 bps does not do well as markets may rise due to above-average earnings or positive comments by the Federal Reserve, among other macro events.

![image](https://user-images.githubusercontent.com/66137235/233874487-1d308e54-a87f-4b28-a6f5-4fe18f2e8923.png)

The image above shows the returns if only the market rises by 0.25 bps and we sell expecting it to decline. This strategy does not do well as there is likely a good reason why markets rise. Above average earnings, positive comments by the Federal Reserve, or other macro events could push markets higher without a loss of momentum. 

![image](https://user-images.githubusercontent.com/66137235/233875069-686b1354-5e13-4c6f-9eaf-34d9ea369b31.png)

Lastly, the return of the SPY since 2012 has been approximately 30%, making it a challenging benchmark to surpass.


{'arith mean': -0.009080294698614636,

 'arith mean (ann)': -2.2882342640508884,
 
 'sigma': 0.4644082828654136,
 
 'sigma (ann)': 7.372252939562539,
 
 'alpha': -0.00024432987974454967,
 
 'alpha SE': 0.00023792144708560865,
 
 'alpha (ann)': -0.06157112969562652,
 
 'alpha SE (ann)': 0.05995620466557338,
 
 'beta': 0.011777518929992337,
 
 'betaSE': 0.007091540426405063,
 
 'Sharpe ratio': -0.01955239609980454,
 
 'Sharpe ratio (ann)': -0.3103846656930723,
 
 'information ratio': -0.0005261100819240921,
 
 'information ratio (ann)': -0.008351738634089795}
 
Upon analyzing the variables, it is evident that the strategy yields a negative alpha in comparison to the returns from the SPY between 10.30 and 13.00. Thus, investing in the S&P 500 would be more favorable than utilizing this strategy. Furthermore, both the arithmetic mean and Sharpe Ratio are negative, which aligns with the negative returns of the trading strategy.

However, the low volatility and beta are expected as the strategy tends to perform well during a gradual decline in the market.

If a quant trader intends to explore this strategy further, they must incorporate a stop loss, optimize the buy and sell times beyond 10.30 and 13.00, and experiment with different values for the 0.25 bps to determine the optimal inputs.
 







