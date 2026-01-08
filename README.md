# Simple MA Crossover Bot (Signal Exits, SMA100 Filter)

This is a simple moving average crossover trading strategy implemented in Pine Script for TradingView.

## Strategy Description

The bot uses two simple moving averages (SMA):
- Fast MA (default 9 periods)
- Slow MA (default 21 periods)

It generates buy signals when the fast MA crosses above the slow MA and price > SMA100, and sell signals when the fast MA crosses below the slow MA and price < SMA100.

Exits positions on reversal signals (long positions exit on sell signals, short positions exit on buy signals).

## Parameters

- **Fast MA Length**: Length of the fast moving average (default: 9)
- **Slow MA Length**: Length of the slow moving average (default: 21)
- **SMA 100 Length**: Length for SMA100 calculation (default: 100)

## Usage

1. Open TradingView in your browser.
2. Navigate to the Pine Editor (found in the bottom panel or via the menu).
3. Copy the contents of `simple_trading_bot.pine` and paste into a new strategy script.
4. Save the script and add it to a chart.
5. Adjust parameters as needed in the script settings.
6. Use TradingView's Strategy Tester to backtest on historical data.
7. For automation:
   - Set alerts on the buy/sell signals.
   - Connect to a supported broker via TradingView's brokerage integrations for automated execution (if available).

## Risk Warning

This bot is for educational and testing purposes only. Trading cryptocurrencies or other assets involves significant risk of loss. Always backtest strategies thoroughly and never risk more than you can afford to lose. Consult a financial advisor before using in live trading.

## Files

- `simple_trading_bot.pine`: The Pine Script strategy file.
