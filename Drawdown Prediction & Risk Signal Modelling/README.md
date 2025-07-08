# Drawdown Prediction & Risk Signal Modelling

**Simulated a systematic risk signal to flag multi-day drawdowns >5%, enabling proactive downside protection and dynamic capital-at-risk control.**

## Project Objective

This project builds a predictive risk signal using supervised learning to anticipate large portfolio drawdowns (20-day return < -5%) across diversified ETF allocations. The objective is to provide early-warning diagnostics and dynamic portfolio risk overlays suitable for systematic strategies.

## Methodology

- **Signal Construction**: Trained a logistic regression model on lagged return features, realized volatility, and historical drawdown patterns to classify risk events. Achieved 100% sensitivity and AUC 0.98 on out-of-sample test data.
  
- **VaR/ES Stress Benchmarking**:
  - Compared **parametric**, **historical**, and **Monte Carlo** risk measures across ETF portfolios with varying concentration and diversification levels.
  - Highlighted tail risk characteristics and capital-at-risk under simulated market shocks.

- **Visualization & Reporting**:
  - Created rolling risk surfaces and drawdown forecast zones.
  - Mapped projected outcomes to dynamic risk budget constraints for fund oversight teams.

- **Pipeline & Stack**:
  - Built an end-to-end Python pipeline using `scikit-learn`, `statsmodels`, and `matplotlib` for signal generation, backtesting, and risk report automation.
  - Owned the full stack from **data wrangling** to **signal deployment**, simulating workflows in quant portfolio risk surveillance teams.

## Key Takeaways

- Demonstrates ability to translate market stress periods into predictive features and classification frameworks.
- Connects signal outputs to actionable portfolio overlays, with interpretability for risk officers and systematic PMs.
- Offers a replicable foundation for integrating statistical drawdown forecasting into multi-asset allocation mandates.

## Tools & Libraries

`Python`, `scikit-learn`, `statsmodels`, `matplotlib`, `numpy`, `pandas`, `seaborn`

---

This project reflects real-world quant workflows: from signal hypothesis, through supervised training and stress testing, to reporting. Built to mirror how risk-aware strategies are evaluated and deployed in institutional settings.
