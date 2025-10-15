# Project: Stock Sentiment Analysis Engine 📈

**Version:** 1.0 (File-Based Implementation)
**Last Updated:** 16 October 2025
**Author:** [Your Name/Team]
**Status:** Phase 1 Complete - Proof of Concept

---

## 1.0 Project Overview

This document outlines the technical specifications, current implementation, and future roadmap for the Stock Sentiment Analysis Engine.

The primary objective of this project is to quantify public sentiment from social media and forum discussions regarding a specific publicly traded company and to analyze its correlation with the company's stock market performance. By processing textual data, we generate a daily sentiment score which is then plotted against historical stock prices to visually inspect potential relationships between public "hype" and financial metrics.

### 1.1 Core Methodology
The current implementation operates as a proof-of-concept using a static, pre-collected dataset. The workflow is as follows:
1.  **Ingest** post data from a local CSV file.
2.  **Analyze** the sentiment of each post title using the VADER NLP model.
3.  **Fetch** corresponding historical stock data from Yahoo Finance.
4.  **Aggregate** daily sentiment scores.
5.  **Merge & Visualize** the sentiment trend against the stock's closing price.

### 1.2 Technology Stack
* **Language:** Python 3.9+
* **Core Libraries:**
    * `pandas`: Data manipulation and analysis.
    * `yfinance`: Fetching historical stock market data.
    * `nltk (VADER)`: Sentiment analysis of social media text.
    * `matplotlib` & `seaborn`: Data visualization.
* **Environment:** Jupyter Notebook

---

## 2.0 Technical Documentation

This section details the setup and step-by-step workflow of the current implementation.

### 2.1 Prerequisites & Setup
To run this analysis, the following Python libraries must be installed:

```bash
pip install pandas yfinance nltk matplotlib seaborn jupyterlab