# TWAP-Based Order Execution Engine | ASX DMA Simulator

This project builds a Python-based simulator for modeling TWAP (Time-Weighted Average Price) order slicing and benchmarking execution performance under realistic market constraints. It mirrors institutional DMA (Direct Market Access) behavior, allowing for empirical study of fill quality, slippage, and strategy-to-outcome alignment.

## Objective

To create an execution testing environment for:
- Evaluating TWAP slicing logic under latency and volume constraints
- Measuring execution metrics like implementation shortfall, realized slippage, and efficiency ratios
- Bridging execution *intent* with realized *PnL*

## Key Features

- **TWAP Order-Splitting Framework**: Models institutional-style execution over time slices with configurable trading windows and execution frequency.
- **Microstructure-Aware Simulation**: Implements per-second fills using probabilistic fill modeling and dynamic order book replication under varying volume/latency scenarios.
- **Execution Metrics Analysis**:
  - Implementation Shortfall (IS)
  - Realized Slippage
  - Execution Efficiency Ratios
- **Visualization & Dashboards**: Uses Plotly to build dashboards displaying cost breakdowns, fill curves, and efficiency histograms across simulated regimes.
- **PnL Attribution**: Maps execution decisions to realized PnL, supporting alpha decay studies and post-trade evaluation.

## Tech Stack

- Python (Pandas, NumPy)
- Plotly for dashboarding
- Custom fill probability & slippage logic
- Modular structure for future integration with order book snapshots

## Insights Simulated

- Trade timing impact on execution cost under thin vs. deep markets
- Sensitivity of slippage to order urgency and volume participation
- Strategy outcome drift in presence of latency and market noise

## Why It Matters

This simulator reflects how execution algorithms are stress-tested in real firms to ensure performance holds in live markets. It demonstrates ability to not only build logic, but validate it empirically, a critical step in robust signal-to-execution pipelines.

---

**This project was independently developed to simulate institutional execution pipelines and provide a sandbox for research-grade strategy testing and PnL diagnostics.**
