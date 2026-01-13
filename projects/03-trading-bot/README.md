# Trading Bot (Backtesting + Futures API/WebSockets)

This project is a skills-focused demonstration of my Python engineering and quantitative finance workflow: a research-style futures backtesting notebook and a real-time exchange API prototype using WebSockets and asyncio.

> **Disclaimer:** This repository is for educational/research purposes. The API notebook uses **Binance Futures testnet** and is **not financial advice**.

## What this project demonstrates
- **Python engineering:** class-based design and reproducible notebook workflow
- **Market data processing:** historical data extraction and structured analysis
- **Real-time streaming:** WebSocket market data with `asyncio`
- **Exchange API integration:** account checks, leverage settings, and order placement (testnet)
- **Strategy evaluation:** vectorized return computation and performance visualization

## Notebooks
### 1) `backtesting.ipynb` — Futures Strategy Backtesting (Leverage & Costs)
Research-style backtesting of a rule-based long/short strategy:
- vectorized performance calculation
- transaction cost approximation
- leverage sensitivity experiments and equity-curve comparison

**Limitations:** simplified execution assumptions (bar-based fills), no slippage model; parameter exploration is for hypothesis generation.

### 2) `futures_with_api.ipynb` — Futures API + Real-Time Streaming (Testnet)
Hands-on exchange API work demonstrating:
- futures account and trading-mode checks (margin/leverage/positions)
- historical kline data retrieval
- real-time price streaming via WebSockets (`BinanceSocketManager`)
- a minimal trader prototype (stream → signal → execute) on **testnet**

**Limitations:** reliability layer (reconnect/idempotency/logging) is not production-grade.

## How to run (high level)
1. Open the notebooks in Jupyter or VS Code.
2. Install dependencies:
   - `numpy`, `pandas`, `matplotlib`, `python-binance`
3. Use Binance Futures **testnet** API credentials (do not use live keys).
4. Run the notebooks top-to-bottom.

## Next steps (planned improvements)
- Walk-forward / time-split validation for more realistic evaluation
- Risk controls (max position size, stop logic, kill switch)
- Execution reliability (reconnect, retries, order idempotency, structured logging)
