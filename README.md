# Intraday Rush EA - ReadMe

This ReadMe file provides information on how to use the Intraday Rush EA code. Please note that Forex Robot Easy Team is the developer of this code, and for detailed reviews and trading results, please visit the [official website](https://forexroboteasy.com/forex-robot-review/intraday-rush-review-multi-symbol-forex-software-now-95/).

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Trading Parameters](#trading-parameters)
5. [How it Works](#how-it-works)
6. [Error Handling](#error-handling)
7. [Trade Events](#trade-events)
8. [Chart Events](#chart-events)
9. [Disclaimer](#disclaimer)

## Introduction <a name='introduction'></a>
The Intraday Rush EA is a multi-symbol forex trading software. It uses the RSI (Relative Strength Index) indicator to make trading decisions based on overbought and oversold levels. This code is provided as a sample and is not developed or maintained by Forex Robot Easy Team. For official information and support, please refer to the official MQL5 documentation and the developer of this product.

## Prerequisites <a name='prerequisites'></a>
To use this EA code, you need to have a MetaTrader 5 terminal installed on your computer. You also need to have basic knowledge of forex trading and how to use Expert Advisors.

## Installation <a name='installation'></a>
1. Open your MetaTrader 5 terminal.
2. Go to 'File' > 'Open Data Folder' to open the data folder.
3. Copy the EA code file (`.mq5` or `.mqh`) to the 'MQL5' > 'Experts' or 'Indicators' folder.
4. Restart the MetaTrader 5 terminal.
5. The Intraday Rush EA should now be available in the 'Navigator' window under the 'Expert Advisors' section.

## Trading Parameters <a name='trading-parameters'></a>
The following trading parameters can be adjusted in the code:

- `RSI_PERIOD`: The period used for the RSI indicator.
- `RSI_OVERBOUGHT`: The overbought level for the RSI indicator.
- `RSI_OVERSOLD`: The oversold level for the RSI indicator.

These parameters can be modified to suit your trading strategy and risk tolerance.

## How it Works <a name='how-it-works'></a>
1. The code includes the required libraries and modules for trading and the RSI indicator.
2. Symbol constants are defined for the different currency pairs.
3. Trading parameters are set, including the RSI period, overbought level, and oversold level.
4. Instances of the RSI indicator and trade class are created.
5. The `OnInit` function is called during initialization to set up the RSI parameters.
6. The `OnDeinit` function is called during deinitialization to clean up any open trades.
7. The `OnTick` function is called on each tick to check RSI values for each symbol and make trading decisions.
8. Trades are opened based on the RSI values and the defined overbought and oversold levels.
9. The `OnTradeError`, `OnTrade`, and `OnChartEvent` functions are custom functions to handle errors, trade events, and chart events respectively.

## Error Handling <a name='error-handling'></a>
The `OnTradeError` function handles any trade errors and prints the error message.

## Trade Events <a name='trade-events'></a>
The `OnTrade` function can be used to handle trade events. This function can be customized to perform specific actions based on trade events.

## Chart Events <a name='chart-events'></a>
The `OnChartEvent` function can be used to handle chart events. This function can be customized to perform specific actions based on chart events.

## Disclaimer <a name='disclaimer'></a>
Please note that Forex Robot Easy Team is not the official developer of this product. This ReadMe file provides a sample code that can work as described in the product. For official information and support, please refer to the official MQL5 documentation and the developer of this product.
