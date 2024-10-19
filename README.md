# Simulation Model for Options Gamma Hedging

## Overview

This repository contains the implementation of a **Gamma Hedging Simulation Model** developed as part of an independent study. The model simulates options trading strategies with a focus on gamma hedging, allowing traders to test and optimize their hedging actions in advance using predefined parameters.

Gamma hedging is a risk management strategy used in options trading to maintain a delta-neutral position by continuously rebalancing the underlying stock position. This simulation model is designed specifically for **plain-vanilla equity options** and uses the **Black-Scholes Option Pricing Model** for option valuation.

### Key Features
- **Simulation of Gamma Hedging Strategies**: Evaluate the performance of different gamma hedging strategies over a predefined period using Monte Carlo simulations.
- **Customizable Parameters**: Set hedge frequency, stop-loss levels, target-gain levels, and option rolling mechanisms for multiple consecutive trades.
- **Profit and Loss (P&L) Evaluation**: Analyze the P&L of different hedging scenarios, including the time the strategy remains outstanding.
- **Monte Carlo Simulations**: Generate thousands of stock price trajectories to assess various hedging strategies under different market conditions.

### Methodology
The simulation model uses **Monte Carlo methods** to generate stock price paths, evaluates the performance of the hedging strategies, and compares the results for different scenarios. The model focuses on:
- Hedging frequency (daily, weekly, monthly)
- Stop-loss and target-profit levels
- Multiple consecutive option rolls for medium- to long-term strategies

### Requirements
- **R** (for running the simulations)
- **RQuantlib** package (for option pricing calculations)
- **sde** package (for Geometric Brownian Motion simulations)

### How to Use
1. Set the simulation parameters, including the number of simulations, option strike price, implied volatility, hedge frequency, and stop/target levels.
2. Run the simulation to generate stock price paths and option P&L.
3. Analyze the results to determine which gamma hedging strategy performs best under different market conditions.

### Results
The model shows how adjusting hedge frequency and stop/target limits impacts the distribution of P&L and the duration of the strategy. More frequent hedging tends to keep trades alive longer but may limit potential profits, while less frequent hedging can result in higher P&L swings.

### Conclusion
This simulation model helps traders to make more informed hedging decisions by allowing them to test their strategies in a simulated environment before committing to real trades.

## License
This project is licensed under the MIT License.
