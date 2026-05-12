# 📊 News Sentiment Analysis and Stock Market Correlation

This project analyzes the relationship between financial news sentiment and stock market movements using technical analysis indicators and sentiment analysis techniques.

The workflow includes:
- Stock price preprocessing and technical analysis
- Financial news sentiment scoring
- Correlation analysis between sentiment and stock returns
- Data visualization and interpretation

---

# 📁 Project Structure

```text
news-sentiment-analysis/
│
├── data/
│   └── raw/
│       ├── AAPL.csv
│       ├── AMZN.csv
│       ├── GOOG.csv
│       ├── META.csv
│       ├── NVDA.csv
│       └── raw_analyst_ratings.csv
│
├── notebooks/
│   ├── task1.ipynb
│   ├── task2.ipynb
│   └── task3.ipynb
│
├── src/
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

# 📦 Dataset Description

## Stock Price Data
Historical stock datasets were used for:
- Apple (AAPL)
- Amazon (AMZN)
- Google (GOOG)
- Meta (META)
- NVIDIA (NVDA)

### Expected Columns
Each stock CSV file should contain:

```text
Date, Open, High, Low, Close, Volume
```

---

## Financial News Dataset

The project uses a financial news headline dataset:

```text
raw_analyst_ratings.csv
```

### Expected Columns

```text
headline, date
```

---

# ⚙️ Environment Setup

## 1. Clone Repository

```bash
git clone <repository-url>
cd news-sentiment-analysis
```

---

## 2. Create Virtual Environment

### Windows
```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / macOS
```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Download NLTK Resources

Run once inside Python:

```python
import nltk
nltk.download('vader_lexicon')
```

---

# 🚀 Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Then open notebooks from the `notebooks/` directory.

---

# 📈 Task Overview

## Task 1 — Exploratory Data Analysis
- Data cleaning
- Missing value handling
- Initial stock data exploration

---

## Task 2 — Technical Analysis
Computed indicators using TA-Lib and PyNance:
- SMA
- EMA
- RSI
- MACD
- Returns and volatility analysis

Visualizations include:
- Moving averages
- RSI charts
- MACD analysis

---

## Task 3 — Sentiment Correlation Analysis

### Workflow
- Financial news sentiment scoring using VADER
- Date alignment between news and trading days
- Daily return calculation
- Pearson correlation analysis
- Scatter plot visualization
- Sentiment category return analysis

---

# 🧠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- TA-Lib
- PyNance
- NLTK VADER
- SciPy

---

# 📊 Example Analysis Outputs

The project generates:
- Technical indicator visualizations
- Sentiment vs return scatter plots
- Correlation comparison tables
- Average return by sentiment category charts

---

# ⚠️ Limitations

- Sentiment analysis may not fully capture financial context
- Market movement depends on multiple external factors
- News effects may occur with delayed reactions
- Shared news datasets may dilute company-specific sentiment impact

