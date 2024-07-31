## Introduction

This project analyzes Ethereum cryptocurrency data obtained from Binance. The dataset includes comprehensive information on Ethereum trades, including timestamps, opening and closing prices, high and low prices, trading volumes, and additional trade-specific details. The purpose of this analysis is to gain insights into Ethereum's price movements and trading patterns.

### Dataset Overview

The dataset is taken Binance website (https://www.binance.com/en/landing/data) and contains the following columns:

- `open_time`: Timestamp of the opening time of the trade (in unix time format)
- `Open Price`: Price of Ethereum at the opening of the trade
- `High Price`: Highest price of Ethereum during the trade
- `Low Price`: Lowest price of Ethereum during the trade
- `Close Price`: Price of Ethereum at the closing of the trade
- `Volume`: Total volume of Ethereum traded
- `close_time`: Timestamp of the closing time of the trade
- `Quote Asset Volume`: Volume of the quote asset traded
- `Number of Trades`: Total number of trades executed
- `Taker buy base asset volume during this period`: Volume of base asset bought by takers during the trade period
- `Taker buy quote asset volume during this period`: Volume of quote asset bought by takers during the trade period

This analysis will help to understand the market dynamics of Ethereum and make informed decisions based on historical data trends.

### Project Goals

The primary goals of this analysis are to:

- Visualize Ethereum's Price Trends: Explore the historical price movements of Ethereum and identify patterns or trends.
- Analyze Trading Volume: Examine the volume of trades and how it correlates with price changes.
- Identify Trading Opportunities: Use the data to highlight potential trading opportunities based on historical patterns.
- This project aims to provide a comprehensive understanding of Ethereum's market behavior, which can be valuable for traders, investors, and anyone interested in the cryptocurrency market.

### Process

- In the dataset, the timestamps are recorded in minutes. To analyze general trends, I grouped the data into 15, 30, 60, and 120-minute intervals. This aggregation allows for a clearer overview of broader market trends by smoothing out short-term fluctuations.

- In the dataset, the timestamps are recorded in minutes. To analyze general trends, I grouped the data into 15, 30, 60, and 120-minute intervals. For each time interval, the opening price, closing price, high price, and low price were determined, and the total volume was calculated. Additionally, the percentage change in price was calculated. This aggregation allows for a clearer overview of broader market trends by smoothing out short-term fluctuations.

  ### Outcomes

- I created a graph that shows the volume versus percentage price change for each time interval. This visualization helps to identify the relationship between trading volume and price movements over different periods. For example, there is a volume vs. price change graph for a 120-minute interval. When there is a low price change, the volume is below 200 million dollars. When we look at the graph, we see that when the price change is over or under 2.5%, the volume increases dramatically. Therefore, strategies that operate in high-volume order books should consider these price changes.
  
  ![png-1](https://github.com/user-attachments/assets/ee1efa89-e5d8-4cdf-a05e-acbf6f17ad63)

- A taker buy order is a market order where the buyer agrees to purchase at the current market price, removing liquidity from the market.
- A taker sell order is a market order where the seller agrees to sell at the current market price, also removing liquidity from the market.
- When examining the data and the graph, it is observed that taker buy and taker sell orders each constitute approximately 50% of the total trading volume. This balance suggests a relatively equal distribution of buying and selling pressure in the market.

- When we look at the 6-month Ethereum price and its changes, we see that the highest value is 4091 dollars. We know that it has reached this point 5 times, so this point is a resistance level for us. In the future, when it reaches these levels, we can say that investors holding positions should be cautious, as there is a high probability of a reversal from this point.
- Similarly, when we look at the 6-month chart, we see that the lowest value was in January. However, the price has not fallen to those levels again but has reached a local minimum of 2750 to 3000 dollars 19 times. These points can also be seen as support levels for long-term investors.
  
![png-2](https://github.com/user-attachments/assets/6763227f-ff6f-4757-9cc4-5df229198f8f)

- Using the 6-month row data obtained from Binance, we converted minute-level data into a 120-minute candlestick chart and examined price volatility and volume changes during this period. By analyzing this chart, we can interpret the previously studied volume-price relationship as follows: We observed that volume increased during periods of price volatility. Here, we saw that the volume increase during price uptrends is more obvious. Based on this information, we can consider that an increase in volume for a coin might be an indication of a buying signal.

![png-3](https://github.com/user-attachments/assets/49cd2828-09c7-4b5f-b87a-41d33caac74a)

- Using the raw data, we created graphs for the 15-minute, 60-minute, and 120-minute moving average prices. Since our data spans 6 months, I focused on the one-month segment from June for better clarity. On these graphs, I examined the points where the moving average lines intersected and the subsequent price changes. Generally, I observed that when a shorter moving average crosses above a longer moving average from below, an uptrend often begins. Conversely, when the shorter moving average crosses below the longer moving average, a downtrend typically starts.
  
![png-4](https://github.com/user-attachments/assets/79423e59-9330-480c-b231-3e5f3df6085a)
