# Black Bird MT4

**Developer:** Forex Robot Easy Team

**Developer's Site:** [forexroboteasy.com](https://forexroboteasy.com)

This code is an implementation of the Black Bird MT4 Expert Advisor. The Expert Advisor is designed to perform technical analysis and market pattern detection in order to identify market entry opportunities. It uses moving averages and other technical indicators to make trading decisions.

## Input Parameters

- TakeProfit: Take profit in pips (default: 50.0)
- StopLoss: Stop loss in pips (default: 30.0)
- LotSize: Lot size for trades (default: 0.1)

## Global Variables

- trade: Trade object for executing trades

## Initialization

The `OnInit()` function is called when the Expert Advisor is initialized. In this function, trade parameters are set using the `trade` object. The expert magic number is set to 123456 and the deviation in points for order execution is set to 10.

## Trading Logic

The `OnTick()` function is called on each tick of the market. This is where the trading logic is executed. First, technical analysis and market pattern detection is performed. Then, the code checks for market entry opportunities using specific conditions. If a condition for a buy trade is met, a new trade is opened using the `trade.Buy()` function. If a condition for a sell trade is met, a new trade is opened using the `trade.Sell()` function.

## Trade Events

The `OnTrade()` function is called when trade events occur. It checks if any trades are open using the `trade.PositionSelect()` function. If a trade is open, it checks for conditions to close the trade using the `trade.PositionClose()` function.

## Deinitialization

The `OnDeinit()` function is called when the Expert Advisor is deinitialized. Currently, there is no clean up required for this code.

---

This code is a sample implementation of the Black Bird MT4 Expert Advisor. It is not the official version of the product developed by Forex Robot Easy Team. The official developer of this product can be found using MQL5.

For detailed reviews and trading results of the official Black Bird MT4 Expert Advisor, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/black-bird-mt4-review-advanced-forex-software-for-low-risk-trading/).
