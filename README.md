<div align="center">

<h1>AI-Powered Market Trend Forecasting & Dynamic Pricing System</h1>

<p>A comprehensive, multi-page Streamlit dashboard for retail sales analysis — clean data, segment customers, forecast demand using deep learning, and receive AI-driven pricing recommendations.</p>

<p>
  <img src="https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python" alt="Python">
  <img src="https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=flat-square&logo=streamlit" alt="Streamlit">
  <img src="https://img.shields.io/badge/Deep%20Learning-LSTM%20%7C%20GRU-purple?style=flat-square" alt="Deep Learning">
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square" alt="License">
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

```
📦 project-root/
├── app.py                    # Main entry point — UI layout & tab routing
├── data_processing.py        # Data loading, cleaning & preprocessing pipeline
├── eda.py                    # Business overview tab functions
├── customer_segmentation.py  # RFM & K-Means segmentation logic
├── forecasting.py            # LSTM & GRU model pipeline
├── dynamic_pricing.py        # Price simulation & revenue optimization
├── utils.py                  # Shared utilities & plot color palette
└── requirements.txt          # Python dependencies
```

---

## Setup & Installation

### Prerequisites

- Python **3.8** or newer
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
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`.

---

## Deployment

This project is ready for deployment on **Streamlit Community Cloud**.

| Step | Action |
|------|--------|
| 1. Push to GitHub | Upload all `.py` files and `requirements.txt` to a public repository |
| 2. Connect | Sign in at [share.streamlit.io](https://share.streamlit.io) with your GitHub account |
| 3. Deploy | Click **New app** → select your repository → set main file to `app.py` → click **Deploy!** |

Streamlit Cloud will automatically install dependencies from `requirements.txt` and host the app at a shareable URL.

---

<div align="center">
  <sub>Built with Streamlit · PyTorch · scikit-learn · Plotly</sub>
</div>
