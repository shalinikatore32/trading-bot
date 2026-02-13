# Simplified Trading Bot – Binance Testnet

## 📌 Overview

This is a CLI-based Python trading bot that places MARKET and LIMIT orders on Binance Testnet.

The application follows a clean, modular structure with:

- Separate client layer
- Order execution layer
- Input validation layer
- Logging configuration
- Structured CLI interface
- Exception handling

---

## 🛠 Tech Stack

- Python 3.x
- python-binance
- argparse (CLI)
- logging module

---

## 📂 Project Structure

trading_bot/
│
├── bot/
│ ├── client.py # Binance client configuration
│ ├── orders.py # Order placement logic
│ ├── validators.py # Input validation
│ ├── logging_config.py
│
├── cli.py # CLI entry point
├── requirements.txt
├── trading_bot.log # Log file (generated after execution)
└── README.md

---

## ⚙️ Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/shalinikatore32/trading-bot.git
cd trading-bot
```

## 2️⃣ Create Virtual Environment

```bash
python -m venv venv
venv\Scripts\activate

```

## 3️⃣ Install Dependencies

```bash

3️⃣ Install Dependencies
```

## 4️⃣ Create .env File

```bash

```

BINANCE_API_KEY=your_api_key_here
BINANCE_API_SECRET=your_secret_here

```

```

## ▶️ How to Run

- 🔹 MARKET Order Example

```bash
python cli.py --symbol BTCUSDT --side BUY --type MARKET --quantity 0.001


```

- 🔹 LIMIT Order Example

```bash
python cli.py --symbol BTCUSDT --side SELL --type LIMIT --quantity 0.001 --price 70000

```

## 📄 Example Output

```bash
=== ORDER REQUEST SUMMARY ===
Symbol: BTCUSDT
Side: BUY
Type: MARKET
Quantity: 0.001

=== ORDER RESPONSE ===
Order ID: 1920055
Status: FILLED
Executed Qty: 0.00100000

✅ Order placed successfully!

```

## 📌 Assumptions

- Valid API credentials are configured
- User has sufficient testnet balance
- Symbol provided exists on Binance Testnet
