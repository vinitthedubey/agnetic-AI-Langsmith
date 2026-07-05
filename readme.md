# 📈 AI Stock Analysis & Recommendation System

An AI-powered Stock Analysis application built using **Google ADK**, **Google Gemini**, **LangSmith**, **Machine Learning**, and **Yahoo Finance**.

The application analyzes historical stock prices, technical indicators, recent market news, and sentiment to predict future stock prices and generate BUY/HOLD/SELL recommendations.

The project is instrumented with **LangSmith** for tracing and monitoring and is intended to demonstrate **Fleet's On-Call Copilot** capabilities for AI application incident investigation.

---

# Features

- Historical stock data using Yahoo Finance
- Technical Indicators
    - SMA
    - EMA
    - RSI
    - MACD
    - Bollinger Bands
- News Retrieval using Google News RSS
- Sentiment Analysis using VADER
- Machine Learning Prediction using Random Forest
- Time Series Forecast using Prophet
- AI Recommendation using Google Gemini
- LangSmith tracing
- Google ADK Agent Workflow
- Incident investigation support using Fleet On-Call Copilot

---

# Architecture

```
                User
                  │
                  ▼
          Stock Analysis Agent
                  │
                  ▼
            Data Agent
                  │
                  ▼
            News Agent
                  │
                  ▼
       Sentiment Analysis Agent
                  │
                  ▼
     Technical Indicator Agent
                  │
                  ▼
      Random Forest Prediction
                  │
                  ▼
        Prophet Forecast Agent
                  │
                  ▼
     Recommendation Agent (Gemini)
                  │
                  ▼
              Final Report
```

---

# Technology Stack

| Component | Technology |
|------------|------------|
| Programming Language | Python |
| Notebook | Jupyter |
| Agent Framework | Google ADK |
| LLM | Gemini 2.5 Flash |
| Monitoring | LangSmith |
| Stock Data | Yahoo Finance |
| News | Google News RSS |
| Sentiment | VADER |
| ML Model | Random Forest |
| Forecasting | Prophet |
| Visualization | Matplotlib |

---

# Repository Structure

```
.
├── notebook.ipynb
├── README.md
├── requirements.txt
├── runbooks/
│   ├── INVALID_TICKER.md
│   ├── DATA_DOWNLOAD_FAILURE.md
│   ├── GEMINI_API_FAILURE.md
│   ├── NEWS_FETCH_FAILURE.md
│   ├── PREDICTION_AGENT_FAILURE.md
│   └── HIGH_LATENCY.md
```

---

# Workflow

1. User enters stock ticker

2. Download one year historical data

3. Fetch latest market news

4. Perform sentiment analysis

5. Generate technical indicators

6. Predict future stock price

7. Forecast using Prophet

8. Generate BUY / HOLD / SELL recommendation

9. Store execution traces in LangSmith

---

# LangSmith Integration

LangSmith is used to monitor every workflow execution.

Captured metrics include:

- Agent execution
- LLM calls
- Prompt
- Response
- Token usage
- Latency
- Errors
- Exceptions
- Trace visualization
- Workflow graph

---

# Fleet On-Call Copilot Integration

This project is used to evaluate Fleet's On-Call Copilot.

The Copilot investigates incidents using:

- LangSmith traces
- GitHub repository
- Runbooks
- README
- Slack
- Incident history

Expected outputs:

- Incident summary
- Root cause analysis
- Suggested resolution
- Draft ticket
- Draft Slack update

---
