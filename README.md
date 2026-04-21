<h1 align="center">BITSCOPE 🪙</h1>
<p align="center">
<b>Advanced Bitcoin Sentiment Correlation & Price Estimation System</b>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/FinBERT-Sentiment-blue?style=for-the-badge"/>
<img src="https://img.shields.io/badge/XGBoost-Regressor-green?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Streamlit-App-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
</p>

---

## 📈 Overview

**BITSCOPE** is a financial intelligence tool designed to quantify the "fear and greed" of the cryptocurrency market. By scraping real-time news and social data and processing it through specialized **Natural Language Processing (NLP)** models, BITSCOPE correlates public sentiment with Bitcoin price movements to provide actionable insights.

Unlike general sentiment tools, BITSCOPE is optimized for financial vocabulary, allowing it to detect subtle market signals that standard models miss.

---

## 🏗️ System Architecture

The project is built as a modular pipeline, separating data acquisition from model inference:

| Directory | Component | Description |
|-----------|-----------|-------------|
| `scraper/` | **Data Ingression** | Automated scripts to fetch headlines and social signals. |
| `models/` | **Intelligence** | Pre-trained FinBERT weights and XGBoost regression models. |
| `notebooks/`| **Research** | Exploratory Data Analysis (EDA) and model validation. |
| `data/`    | **Storage** | Managed datasets for historical price and sentiment logs. |
| `app.py`   | **Interface** | Streamlit dashboard for real-time visualization. |

---

## ⚙️ The Pipeline

1. **Extraction**: Automated scrapers gather the latest Bitcoin-related news from high-authority sources.
2. **NLP Processing**: Text data is passed through **FinBERT**, a BERT model specifically pre-trained on financial corpora, to generate high-accuracy sentiment scores.
3. **Correlation Logic**: Sentiment scores are merged with OHLCV (Open, High, Low, Close, Volume) market data.
4. **Price Estimation**: An **XGBoost Regressor** analyzes the combined features to estimate potential short-term price trends.
5. **Real-time UI**: Insights are rendered onto an interactive Streamlit dashboard.

---

## 🚀 Key Features

- **Specialized Sentiment Analysis**: Uses FinBERT to understand financial context (e.g., distinguishing "inflation" from "growth").
- **Volatility Mapping**: Visualizes how sharp drops in sentiment precede price corrections.
- **Automated Scraping**: Continuous data collection to keep predictions current.
- **Interactive EDA**: Jupyter notebooks included for deep-diving into historical correlation patterns.

---

## 🛠️ Tech Stack

- **Core**: Python 3.10+
- **Machine Learning**: HuggingFace Transformers, Scikit-learn, XGBoost
- **Data Handling**: Pandas, NumPy, BeautifulSoup4
- **Visualization**: Streamlit, Matplotlib, Plotly

---

## 🏁 Getting Started

### Installation

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Yash6163/BITSCOPE.git](https://github.com/Yash6163/BITSCOPE.git)
   cd BITSCOPE
