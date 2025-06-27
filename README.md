# Metaverse Anomaly Detection in Blockchain Transactions

## Overview

This research project focuses on detecting and predicting anomalies in blockchain transactions within the Open Metaverse using advanced machine learning techniques. By forecasting both the risk score (numerical) and anomaly level (categorical: low, moderate, high), the project presents a robust and insightful approach to understanding transaction-based threats in virtual ecosystems. IBM WatsonX was used for model building, experimentation, and evaluation.

## Dataset

- **Source:** Collected from the Open Metaverse ecosystem involving 200+ companies
- **File:** `metaversedata.csv`
- **Year:** 2022
- **Features:** 14 parameters
- **Target Columns:**
  - `risk_score` (numerical)
  - `anomaly` (categorical - low\_risk, moderate\_risk, high\_risk)

## Objective

To explore different ML pipelines that:

1. Predict the `risk_score` for blockchain transactions.
2. Classify the `anomaly` level based on features.

## Approach

Three categories of algorithmic techniques were employed:

- **Relationship-based** algorithms
- **Window-based** algorithms
- **Forecasting-based** algorithms

An ensemble of these techniques was evaluated using precision, recall, F1-score, average precision, and AUC metrics. The study also explores the interpretability of linear regression variants enhanced with regularization.

## Tools & Libraries

- IBM WatsonX
- Jupyter Notebooks
- Python (NumPy, pandas, scikit-learn, matplotlib)

### WatsonX Pipelines Used:

```
PointwiseBoundedHoltWintersAdditive, PointwiseBoundedBATS,
PointwiseBoundedBATSForceUpdate, WindowNN,
WindowLOF, WindowPCA
```

## Results Summary

### Risk Score Prediction

- **Best Pipeline:** `Pipeline 6 (Relationship)`
- **Top 3 Pipelines:** Pipeline 6, Pipeline 5 (Window), Pipeline 1 (Forecasting)
- **Files:**
  - `riskScoreP6__relationship.ipynb`
  - `riskScoreP5__window.ipynb`
  - `riskScoreP1__forecasting.ipynb`
  - `riskScoreIntegrated.ipynb`

### Anomaly Classification

- **Best Pipeline:** `Pipeline 2 (Forecasting)`
- **Top 3 Pipelines:** Pipeline 2, Pipeline 6 (Relationship), Pipeline 3 (Forecasting)
- **Files:**
  - `anomalyP2__forecasting.ipynb`
  - `anomalyP6__relationship.ipynb`
  - `anomalyIntegrated.ipynb`

## Contributions

This project demonstrates:

- The effectiveness of ensemble learning techniques in anomaly detection.
- Interpretability in machine learning through regularized models.
- A practical application of AI for risk assessment in digital ecosystems.


## Future Work

- Incorporation of deep learning methods for time series analysis.
- Real-time anomaly monitoring dashboards.
- Expansion to include smart contract and NFT-based transactions.



