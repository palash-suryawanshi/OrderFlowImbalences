# Order Flow Imbalances (OFI)

This repository contains the implementation of various Order Flow Imbalance (OFI) features as part of a technical trial task. The objective is to evaluate price impact models and the predictive power of OFI in short-term equity return forecasting.

## 📁 Dataset
- `first_25000_rows.csv` — High-frequency order book data for the stock **AAPL**.

## 📌 Objectives

Implemented the following OFI features:
- ✅ **Best-Level OFI**: Based on the top-of-book bid/ask price and size changes.
- ✅ **Multi-Level OFI**: Aggregates OFI across levels 0–9 of the order book.
- ✅ **Integrated OFI**: Time-integrated OFI over a 1-second rolling window using Best-Level OFI.
- ⛔ **Cross-Asset OFI**: Not implemented due to the dataset containing only a single stock (AAPL). Cross-asset OFI requires synchronized multi-asset data.


## ⚙️ How to Run

1. Clone this repo and open the notebook in Google Colab or Jupyter.
2. Upload the dataset (`first_25000_rows.csv`) to your working directory.
3. Execute each cell to compute the OFI features.
4. Output files (`*.csv`) will be generated and saved for download.

## 📘 Conceptual Summary

Answers to the following questions are included in the LaTeX folder named as `Conceptual Questions and Answers.pdf`:
1. Motivation for multi-level OFI
2. Why Lasso is used over OLS for cross-impact estimation
3. Why OFI is more predictive than trade volume

## 📖 Reference

This work is based on the research paper:  
**Rama Cont, Mihai Cucuringu & Chao Zhang.**  
*Cross-Impact of Order Flow Imbalance in Equity Markets*.

---

