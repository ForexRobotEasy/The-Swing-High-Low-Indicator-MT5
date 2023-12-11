# Swing High Low Indicator ReadMe

This ReadMe file provides information about the Swing High Low Indicator code.

## Description

The Swing High Low Indicator is a custom indicator for MetaTrader 5 (MT5) that identifies swing highs and swing lows in the price chart. A swing high is a candlestick with a higher high than the previous candles, while a swing low is a candlestick with a lower low than the previous candles. The indicator marks the swing highs with blue arrows and the swing lows with red arrows on the price chart.

## Developer

The Swing High Low Indicator was developed by the Forex Robot Easy Team. Forex Robot Easy is a website dedicated to providing information and resources related to forex trading and forex robots. For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/swing-high-low-indicator-mt5-review-optimize-forex-trades-for-2022/). Please note that Forex Robot Easy is not the official developer of this product. To find the official developer of this product, please use MQL5.

## Indicator Settings

- `swingPeriod`: Number of candles for swing calculation. Default value is 10.

## Indicator Parameters

- `swingHighBuffer[]`: Buffer to store swing high values.
- `swingLowBuffer[]`: Buffer to store swing low values.

## Indicator Initialization

The indicator initialization function `OnInit()` is responsible for setting up the indicator buffers and styles. It sets the two indicator buffers `swingHighBuffer` and `swingLowBuffer` for storing swing high and swing low values, respectively. It also sets the indicator colors for the swing highs and swing lows.

## Indicator Calculation

The indicator iteration function `OnCalculate()` is responsible for calculating the swing highs and swing lows based on the input price data. It iterates through the price data and checks if each candle is a swing high or swing low by comparing it with the previous candles within the specified swing period. If a candle is a swing high, its high value is stored in the `swingHighBuffer` and the `swingLowBuffer` is set to `EMPTY_VALUE`. If a candle is a swing low, its low value is stored in the `swingLowBuffer` and the `swingHighBuffer` is set to `EMPTY_VALUE`. The function returns the total number of rates.

## Usage

To use the Swing High Low Indicator, simply add it to a chart in MetaTrader 5. Adjust the `swingPeriod` parameter if needed. The indicator will then display blue arrows for swing highs and red arrows for swing lows on the chart.

Please note that this code is provided as a sample and may need to be modified or optimized for specific trading strategies or requirements.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/swing-high-low-indicator-mt5-review-optimize-forex-trades-for-2022/).
