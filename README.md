

A sophisticated algorithmic trading bot that implements Bollinger Bands strategy for automated trading. The bot integrates with multiple data sources and trading platforms to provide a comprehensive trading solution.

## Features

- **Trading Strategy**: Implements Bollinger Bands-based trading strategy
- **Data Sources**:
  - Yahoo Finance for market data
  - TD Ameritrade integration
  - IEX Cloud for additional market data
- **Trading Platform**: Alpaca for paper trading and live trading
- **Data Storage**: MongoDB for storing calculations and process status
- **Technical Analysis**: Includes TA-Lib for advanced technical analysis
- **Backtesting**: Supports strategy backtesting capabilities

## Prerequisites

- Python 3.8 or higher
- MongoDB
- TA-Lib (Technical Analysis Library)
- API keys for:
  - Alpaca
  - TD Ameritrade
  - IEX Cloud

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/TradingBot.git
cd TradingBot
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Install TA-Lib:
   - For Windows: Use the provided wheel file `TA_Lib-0.4.19-cp38-cp38-win_amd64.whl`
   - For other platforms: Follow the official TA-Lib installation guide

4. Set up your environment variables or configuration file with your API keys:
   - Alpaca API key and secret
   - TD Ameritrade API credentials
   - IEX Cloud API key
   - MongoDB connection string

## Project Structure

```
Python-trading-bot/
├── app/
│   ├── Alpaca/         # Alpaca trading platform integration
│   ├── Components/     # Core trading components
│   ├── Data/          # Data handling and processing
│   ├── IexCloud/      # IEX Cloud integration
│   ├── Mongo/         # MongoDB database operations
│   ├── Other/         # Additional utilities
│   ├── TDA/           # TD Ameritrade integration
│   └── main.py        # Main application entry point
├── requirements.txt    # Python dependencies
└── README.md          # This file
```

## Usage

1. Configure your trading parameters in the appropriate configuration files
2. Run the main application:
```bash
python app/main.py
```

## Features in Detail

### Trading Strategy
- Bollinger Bands implementation for entry and exit signals
- Customizable parameters for band width and period
- Risk management rules

### Data Management
- Real-time market data processing
- Historical data storage and analysis
- MongoDB integration for persistent storage

### Trading Execution
- Paper trading support through Alpaca
- Live trading capabilities
- Order management and position tracking

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Disclaimer

This trading bot is for educational and research purposes only. Use at your own risk. Past performance is not indicative of future results. Always test thoroughly in a paper trading environment before using real money.
