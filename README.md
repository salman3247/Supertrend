# SuperTrend Indicator for MetaTrader 5

A powerful technical analysis tool for MetaTrader 5 that helps identify market trends based on Average True Range (ATR) volatility.

## Description

The SuperTrend indicator plots a line above or below the price action to identify the current market trend. When the indicator line is green and below the price, it suggests an uptrend. When it's red and above the price, it suggests a downtrend. The indicator uses ATR to dynamically adjust to market volatility, making it effective across different timeframes and market conditions.

## Core Formula

- Upper Band = Source Price + (Multiplier × ATR)
- Lower Band = Source Price - (Multiplier × ATR)
- In uptrend: SuperTrend = Lower Band (green)
- In downtrend: SuperTrend = Upper Band (red)

## Features

- Color-coded line for easy trend identification
- Adjustable sensitivity through ATR period and multiplier
- Multiple price source options
- Option to include or exclude price wicks in calculations
- Implements trailing stop logic for dynamic support/resistance levels

## Installation

1. Download the `supertrend.mq5` file
2. Copy it to your MetaTrader 5 indicators folder (typically located at `Terminal_Directory\MQL5\Indicators\`)
3. Restart MetaTrader 5 or refresh the Navigator panel
4. Drag the indicator onto any chart

## Parameters

- **ATRPeriod**: Period for ATR calculation (default: 22)
- **Multiplier**: ATR multiplier to adjust sensitivity (default: 3.0)
- **SourcePrice**: Price type used for calculations (default: PRICE_MEDIAN)
- **TakeWicksIntoAccount**: Whether to include price wicks in calculations (default: true)

## Usage Examples

- **Trend Following**: Enter long when SuperTrend turns green, exit when it turns red
- **Trailing Stop**: Use the SuperTrend line as a dynamic stop-loss level
- **Trend Confirmation**: Combine with other indicators for stronger signals
- **Scalping**: Use on lower timeframes with adjusted parameters for short-term trades

## License

This project is released under the MIT License - see the LICENSE file for details.

## Author

Originally created by Salman Soltaniyan

## Contributing

Contributions, bug reports, and feature requests are welcome! Feel free to submit a pull request or open an issue.

## Disclaimer

This indicator is provided for educational and informational purposes only. Trading involves risk, and past performance is not indicative of future results.