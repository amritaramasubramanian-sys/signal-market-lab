# SIGNAL | Market Intelligence Lab

**Version 2.0** is an interactive educational research sandbox exploring three connected layers of financial markets: probability formation, market pricing, and execution.

## Open the project
Visit the GitHub Pages deployment (after enabling Pages in repository settings), or open `index.html` locally in a modern browser. No build tools, packages, API keys, or external services are required.

## Modules

### 1. Market overview
- Adjust a prior probability, evidence strength, evidence reliability, residual uncertainty, liquidity, and an illustrative market midpoint.
- Compare an evidence-adjusted model estimate with a market-implied probability.
- Inspect a synthetic time series and a plain-language interpretation of model-market disagreement.

### 2. Evidence engine
- Applies a simplified Bayesian update in log-odds space.
- Makes the effect of evidence reliability explicit.
- Includes a source-quality checklist to prompt scrutiny of independence, sample selection, timeliness, and double-counting.

### 3. Market microstructure
- Generates a synthetic five-level bid/ask book.
- Lets users vary a hypothetical order size.
- Demonstrates how displayed depth, liquidity, spread, and estimated slippage interact.

### 4. Forecast lab
- Record a probability forecast before the outcome is known.
- Resolve forecasts and calculate the Brier score.
- Forecast records are stored locally in the user's browser and are not sent to a server.

### 5. Methodology
- Documents the toy model assumptions and limitations.
- Distinguishes model probability, market-implied probability, and transaction costs.

## Model notes and limitations

All market prices, order-book levels, and time-series values are synthetic. The Bayesian evidence signal is a user-controlled illustrative log-likelihood contribution, not one estimated from empirical data. The uncertainty band is a simple symmetric approximation, not a formal posterior credible interval. The execution-impact function is stylized and not calibrated to observed order books.

This prototype is intended to teach critical thinking about assumptions, uncertainty, calibration, and liquidity. It is not a live market terminal, does not predict actual events, and does not provide investment or trading advice.

## Research roadmap
1. Ingest a timestamped, documented historical event-market dataset.
2. Estimate likelihood ratios from independently labeled evidence.
3. Evaluate calibration out of sample with Brier scores, log loss, and reliability diagrams.
4. Compare predicted execution costs with observed order-book depth and realized slippage.
5. Add reproducible notebooks, data provenance, and model versioning.
