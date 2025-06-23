# Delta-Neutral-Hedging
Delta Hedging and Option Pricing using Black-Scholes and GBM
This project demonstrates the implementation of the Black-Scholes-Merton model for option pricing and dynamic hedging strategies on both simulated and real market data. It is divided into two key notebooks:

1. **GBM.ipynb** – Simulation-based hedging using synthetic stock prices generated via Geometric Brownian Motion.
2. **Black Scholes.ipynb** – Application of Black-Scholes-based delta hedging strategies using historical Tesla stock data.

---

## 📘 Part 1: GBM-based Simulation

This notebook walks through:

- Generating synthetic stock price paths using **Geometric Brownian Motion (GBM)**.
- Calculating **Black-Scholes prices** for European Call and Put options.
- Deriving the **Greeks**: Delta, Gamma, Vega, Theta.
- Implementing **delta-neutral hedging** and adjusting the hedge dynamically.
- Simulating the **cash flows**, **option values**, and **portfolio P&L** over time.

Objective: Understand the sensitivity of option hedging performance with respect to price movements, time, and volatility using controlled simulations.

---

## 📗 Part 2: Real Market-Based Delta Hedging

This notebook applies Black-Scholes pricing and delta hedging logic on real Tesla (TSLA) stock prices from 2022 to 2023.

It includes 4 hedging strategies:

1. **Buy Call and Short Stock** – Delta-hedged position to profit from undervalued call.
2. **Sell Call and Long Stock** – Covered call strategy with dynamic hedging.
3. **Buy Put and Long Stock** – Protective put strategy using delta-neutrality.
4. **Sell Put and Short Stock** – Naked put selling hedge.

For each case:

- We price the options using Black-Scholes.
- Analyze **mispricing** (theoretical vs market price).
- Use Greeks to hedge dynamically and rebalance positions daily.
- Track **cash flows**, **stock position**, **portfolio value**, and **final P&L**.

---

## 📦 Requirements

- Python 3.x
- `numpy`, `pandas`, `matplotlib`, `scipy`
- Jupyter Notebook

Install using:
```bash
pip install numpy pandas matplotlib scipy
