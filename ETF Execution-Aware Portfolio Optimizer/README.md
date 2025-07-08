# Execution-Aware ETF Portfolio Optimizer

A research-driven portfolio construction engine designed to simulate live-market constraints, execution slippage, and Sharpe-maximizing allocation logic — built to reflect the practical demands of quant trading and systematic strategy development.

## Objective

This project aims to bridge the gap between traditional portfolio theory and the execution-aware realities of live trading. It delivers a production-style workflow where capital allocation, volatility regimes, and trading frictions interact under stress-tested scenarios — ultimately informing signal-driven decision pipelines.

## Key Components

- **Sharpe-Optimizing Engine**  
  Developed a reusable Python optimizer using `SciPy.optimize` that enforces core-satellite constraints (≥65% core, ≤15% satellite) to replicate institutional allocation logic.

- **Monte Carlo Stress Environment**  
  Simulated 5,000+ volatility-regime paths to evaluate allocation drift, execution lag, tracking error, and stability of Sharpe-max portfolios under stress.

- **Execution Friction Modelling**  
  Incorporated slippage-aware frontier construction with trade lag and error injection to mimic real execution desk frictions and their impact on strategy performance.

- **KPI + Attribution Dashboards**  
  Delivered portfolio diagnostics including drawdown attribution, Sharpe/TE evolution, and KPI benchmarks — reflecting how live strategies are monitored and refined.

## Research Intent

The project simulates how a quant PM or risk team might:

- Translate strategy constraints into convex optimization
- Pre-empt execution bottlenecks through simulation before live deployment
- Stress-test allocations across market regimes to reduce tail fragility
- Bridge research with execution through risk-informed signal infrastructure

## Technologies & Stack

- **Languages**: Python  
- **Libraries**: `NumPy`, `Pandas`, `SciPy`, `Matplotlib`, `Plotly`
- **Methods**:  
  - Constrained mean-variance optimization  
  - Execution-aware frontier mapping  
  - Monte Carlo volatility stress testing  
  - Portfolio KPI diagnostics

