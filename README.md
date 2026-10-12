<div align="center">

<h1>AI-Powered Market Trend Forecasting & Dynamic Pricing System</h1>

<p>A comprehensive, multi-page Streamlit dashboard for retail sales analysis — clean data, segment customers, forecast demand using deep learning, and receive AI-driven pricing recommendations.</p>

<p>
  <img src="https://img.shields.io/badge/Python-3.11-blue?style=flat-square&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=flat-square&logo=streamlit" alt="Streamlit">
  <img src="https://img.shields.io/badge/Deep%20Learning-LSTM%20%7C%20GRU-purple?style=flat-square" alt="Deep Learning">
</p>

<p>
  <a href="https://www.linkedin.com/feed/update/urn:li:activity:7372159137675202561/" target="_blank">
    Watch the Retailytics project walkthrough
  </a>
</p>

</div>

---

## Overview

This system empowers retail businesses to make data-driven decisions by combining exploratory data analysis, customer segmentation, deep learning forecasting, and revenue-optimized pricing — all within a single interactive interface.

---

## Features

### 📊 Business Overview (EDA)

- **Sales Performance** — Visualize trends over time across monthly, daily, and hourly intervals
- **Performer Analysis** — Identify best-selling products, top-performing countries, and underperforming segments
- **Customer & Product Behavior** — Compare new vs. returning customers, track average order value, and run market basket analysis
- **Product Deep Dive** — Select any product for a detailed breakdown of its sales trends and geographical distribution

### 👥 Customer Segmentation

- **RFM Segmentation** — Segment customers by Recency, Frequency, and Monetary value with actionable group insights
- **K-Means Clustering** — Discover non-obvious customer personas using unsupervised machine learning
- **Downloadable Data** — Export segment summaries and enriched transaction data for targeted marketing

### 🔮 Forecasting & Pricing

- **AI Sales Forecasting** — Predict future daily sales per product using LSTM and GRU deep learning models
- **Forecast Breakdown** — Visual summaries including busy-day pie charts and past vs. future comparisons
- **Smart Price Suggestions** — Simulate price points post-forecast to recommend the optimal revenue-maximizing price

---

## Project Structure

```text
project-root/
├── src/
│   ├── app.py                    # Streamlit entry point
│   ├── data_processing.py        # Loading and preprocessing
│   ├── eda.py                    # Sales analysis
│   ├── customer_segmentation.py  # RFM and K-Means
│   ├── forecasting.py            # LSTM and GRU forecasting
│   ├── dynamic_pricing.py        # Pricing simulations
│   └── utilities.py              # Shared presentation utilities
├── retail_sample_2000.xlsx       # Small example upload
├── competitor_prices.csv        # Optional competitor input
└── requirements.txt             # Dependencies used by root setup
```

---

## Setup & Installation

### Prerequisites

- Python **3.11** (matches the included development container)
- Git

### Steps

**1. Clone the repository**

```bash
git clone https://github.com/nareshkumart07/AI-Powered-Sales-Analyzer-And-Forecasting-Tool
cd AI-Powered-Sales-Analyzer-And-Forecasting-Tool
```

**2. Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
# venv\Scripts\activate         # Windows
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Run the application**

```bash
python -m streamlit run src/app.py
```

The app will open in your browser at `http://localhost:8501`. Run the command from the repository root.

### Try the included sample

Upload `retail_sample_2000.xlsx` in the sidebar, then select **Prepare My Data**. Explore the overview and customer segmentation tabs before training a forecast. Uploaded CSV/XLSX files need these exact columns: `Invoice`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `Price`, `Customer ID`, and `Country`.

The sample is intended for a quick walkthrough; forecast quality depends on the amount and continuity of history for the selected product.

---

## Deployment

To configure **Streamlit Community Cloud**, use the repository root for dependencies and `src/app.py` as the entry point. Validate installation and resource limits in your deployment environment before sharing an application demo.

| Step | Action |
|------|--------|
| 1. Push to GitHub | Upload all `.py` files and `requirements.txt` to a public repository |
| 2. Connect | Sign in at [share.streamlit.io](https://share.streamlit.io) with your GitHub account |
| 3. Deploy | Click **New app** → select your repository → set main file to `src/app.py` → click **Deploy!** |

Streamlit Cloud will automatically install dependencies from `requirements.txt` and host the app at a shareable URL.

## Evaluation and limitations

This is an applied ML portfolio project. Forecasts and pricing simulations are experimental outputs, not proven business outcomes. For a defensible case study, record the data period, product selection, preprocessing, chronological train/test split, and model-versus-naive-baseline metrics. This repository does not establish a validated revenue improvement.

Dependencies are currently unpinned. A full clean-environment installation and end-to-end forecast run are still required for reproducibility. No license file is currently included; a license choice should be confirmed before representing the repository as MIT-licensed.

---

<div align="center">
  <sub>Built with Streamlit · PyTorch · scikit-learn · Plotly</sub>
</div>
