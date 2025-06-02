# Triple-EMA-Trading-System
TradingView Pine Script indicator designed for daily timeframe trend trading. It uses a custom enhanced Triple Hull Moving Average (THMA) algorithm, integrated with volatility-based bands, RSI filtering, and clear trend-based signals.

## Features

- Enhanced THMA with weighted EMA smoothing
- ATR-based bands for dynamic volatility insight
- Configurable buy and sell signal logic
- Directional trend coloring
- Optional RSI filter to reduce false positives
- Trend highlighting for visual clarity
- Built-in alerts for buy/sell signals and direction changes

## Input Parameters

| Parameter          | Description                                  |
|--------------------|----------------------------------------------|
| Source             | Price input (default: close)                 |
| Length             | Smoothing period for THMA                    |
| Show Band          | Toggle ATR-based band visualization          |
| Color Trend        | Apply color coding based on trend direction |
| Band Width         | Multiplier for ATR band width                |
| Show Signals       | Display buy and sell signals                 |
| Highlight Trend    | Enable background highlighting               |
| Use RSI Filter     | Enable RSI filter for signal validation      |
| RSI Length         | RSI calculation length                       |
| RSI Overbought     | Upper threshold for RSI                      |
| RSI Oversold       | Lower threshold for RSI                      |
| Arrow Offset       | Distance of signal markers from price        |

## Strategy Logic

**Buy Signal**
- THMA changes from downtrend to uptrend
- RSI is below the overbought threshold (if RSI filter is enabled)

**Sell Signal**
- THMA changes from uptrend to downtrend
- RSI is above the oversold threshold (if RSI filter is enabled)

**Alerts**
- Buy signal trigger
- Sell signal trigger
- THMA direction change

## Usage Instructions

1. Open the Pine Editor on TradingView
2. Paste the script and save
3. Add to a chart using the daily timeframe
4. Adjust inputs based on your asset or preference
5. Set alerts using the built-in alert conditions

## About the Author

Erika Barker  
Miami-based economic data scientist and quantitative strategist with a background in predictive modeling, econometrics, and algorithmic trading.  
Navy veteran and founder of Mercedes and Mcrill, specializing in financial analytics and forecasting systems.

## License

This script is provided for educational and informational purposes. Use at your own risk. No guarantees are provided regarding performance or accuracy

