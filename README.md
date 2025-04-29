
Built by https://www.blackbox.ai

---

```markdown
# Future MT5 Trading System

## Project Overview
The **Future MT5 Trading System** is an automated trading application designed for use with the MetaTrader 5 platform. It employs a robust trading strategy that analyzes market data to enter and exit trades based on technical indicators. The system supports multiple assets and provides a user-friendly graphical interface for real-time monitoring and control of trading operations.

## Installation

To run this project, ensure you have Python installed on your machine. You will also need to install the required dependencies. Follow the steps below to set the application up:

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt  # Make sure to create a requirements.txt based on your environment
   ```

4. **Ensure MetaTrader 5 is installed and running on your system.**

## Usage

To use the trading system, follow these steps:

1. Run the application:
   ```bash
   python painel.py
   ```

2. **Configure your trading setup:**
   - Select the asset (e.g., forex pair) you wish to trade.
   - Specify the timeframe for trading (M1, M5, M15, H1, etc.).
   - Enter the lot size for your trades.

3. **Start the trading bot** by clicking the “Iniciar Robô” button. Monitor the logs to track trading activities.

4. To stop trading, click the “Parar” button. 

## Features
- Multi-asset support for simultaneous trading.
- Real-time market analysis using indicators like RSI, MACD, Bollinger Bands, and more.
- User-friendly GUI built with tkinter for easy navigation.
- Logging system to track trading activities and errors.
- Risk management features, including maximum daily loss parameters.
- Theme toggle for dark/light mode.

## Dependencies
The project requires the following Python libraries:
- `MetaTrader5`
- `numpy`
- `pandas`
- `tkinter` (comes pre-installed with Python's standard library)

Consider creating a `requirements.txt` file for managing dependencies, which you can generate using:
```bash
pip freeze > requirements.txt
```

## Project Structure
Here’s an overview of the key files and their purposes:

```
.
├── estrategia.py         # Trading strategy implementation
├── painel.py             # Main application UI for single asset trading
├── painel_multi.py       # Main application UI for multi-asset trading
├── utils.py              # Utility functions for trading operations
└── log_system.py         # Logging system for tracking operations
```
### Directory Contents
- **estrategia.py**: Contains the `EstrategiaTrading` class which implements the core trading logic.
- **painel.py**: Contains the user interface for single asset trading, facilitating user input and displaying real-time updates.
- **painel_multi.py**: Contains the user interface designed for managing multiple assets with independent controls.
- **utils.py**: Contains utility functions for market analysis, login management, and risk calculations.
- **log_system.py**: Implements logging functionality to keep track of system operations and trading status.

## Conclusion
The Future MT5 Trading System is designed with robustness and user-friendliness in mind, catering to both novice and experienced traders. By setting up the system, traders can automate their strategies and monitor multiple assets with ease.
```