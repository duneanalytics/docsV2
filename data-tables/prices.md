---
description: These tables allow you to get the price of almost all relevant erc20 tokens.
---

# Prices

### Prices from third party data providers <a href="#centralised-exchanges-trading-data" id="centralised-exchanges-trading-data"></a>

We pull price data from the [coinpaprika ](https://coinpaprika.com/)API.

The Price is the volume-weighted price based on real-time market data, translated to USD.

### **prices.usd**

This table supports a range of erc20.tokens.\
If the token you desire is not listed in here, please make a pull request to our [github repository](https://github.com/duneanalytics/abstractions/tree/master/prices).

| **column name**   | **description**                               |
| ----------------- | --------------------------------------------- |
| contract\_address | the contract address of the erc20 token       |
| symbol            | the identifier of the asset (ticker, cashtag) |
| price             | the price of the asset in any given minute    |
| minute            | the resolution for this table is by minute    |

Note that `WETH` can be used for ETH price as it trades at virtually the same price.

### **prices.layer\_1usd**

This table supports layer 1 assets on other blockchains.

| contract\_address | the contract address of the erc20 token       |
| :---------------: | --------------------------------------------- |
|       symbol      | the identifier of the asset (ticker, cashtag) |
|       price       | the price of the asset in any given minute    |
|       minute      | the resolution for this table is by minute    |
