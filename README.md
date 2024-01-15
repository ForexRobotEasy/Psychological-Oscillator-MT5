# Psychological Oscillator MT5 ReadMe

Psychological Oscillator MT5 is a custom indicator developed by the Forex Robot Easy Team. This indicator calculates the psychological oscillator, which measures the ratio of bullish to bearish candles over a specified period. It also generates color histograms and integrates zones based on the oscillator value. The indicator is designed for use on the MetaTrader 5 platform.

## Indicator Inputs

The following inputs can be customized:

- `period`: The period for calculating the psychological oscillator (default: 14)
- `overboughtLevel`: The overbought level (default: 80)
- `oversoldLevel`: The oversold level (default: 20)

## Indicator Buffers

The indicator uses two buffers to store data:

- `HistogramBuffer`: Buffer for storing the histogram values
- `ZoneBuffer`: Buffer for storing the zone values

## Indicator Initialization

The `OnInit()` function is responsible for initializing the indicator. It sets up the indicator buffers, styles, labels, and draw begin points.

## Indicator Calculation

The `OnCalculate()` function is responsible for calculating the indicator values. It loops through the price data and calculates the psychological oscillator, color histograms, and zones for each bar. The calculated values are stored in the indicator buffers.

## Indicator Deinitialization

The `OnDeinit()` function is called when the indicator is removed from the chart. It can be used to clean up any resources if necessary.

## Indicator Inbuilt Notification

The `SendNotification()` function is a placeholder for implementing a notification system. It can be customized to send notifications based on certain conditions or events.

## Indicator Usage Example

The `ExampleUsage()` function demonstrates how to use the indicator. It calculates the psychological oscillator using the `iCustom()` function and performs different actions based on the oscillator value, such as printing bullish/bearish/neutral labels and integrating with trend indicators.

## Indicator Test Function

The `TestIndicator()` function is a placeholder for adding test cases to validate the correctness of the indicator. It can be customized to include specific test scenarios.

## Indicator Execution Entry Point

The `OnTick()` function is the entry point for the indicator's execution. In this example, it calls the `ExampleUsage()` function to demonstrate the usage of the indicator.

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/psychological-oscillator-mt5-a-comprehensive-forex-indicator-review/). To find the official developer of this product, please use MQL5.
