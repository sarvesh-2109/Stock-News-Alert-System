# Stock News Alert System

## Overview

The Stock News Alert System is a Python application designed to monitor stock price changes and provide relevant news updates for specific companies. This application is particularly useful for traders and investors interested in staying updated with the latest market movements and news impacting their stock holdings.

## Features

- Monitors stock prices using the Alpha Vantage API.
- Fetches relevant news articles using the News API when significant price changes are detected.
- Sends alerts with stock price changes and news summaries via SMS using Twilio.

## Prerequisites

- Python 3
- An Alpha Vantage API key.
- A News API key.
- A Twilio account with an auth token and SID.

## Installation and Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/stock-news-alert-system.git
   ```
2. Install required Python packages:
   ```bash
   pip install requests twilio
   ```
3. Obtain API keys from [Alpha Vantage](https://www.alphavantage.co/) and [News API](https://newsapi.org/).
4. Set up a Twilio account and obtain your SID, auth token, and a Twilio phone number.

## Configuration

1. Open the Python script (`main.py`).
2. Replace the `STOCK_API_KEY`, `NEWS_API_KEY`, `TWILIO_SID`, and `TWILIO_AUTH_TOKEN` with your respective API keys and Twilio credentials.
3. Configure the `STOCK_NAME` and `COMPANY_NAME` variables as per your preference.

## Usage

Run the script:

```bash
python main.py
```

If the stock price of the specified company changes significantly (more than 4% in this setup), you will receive an SMS alert with the latest news articles related to that company.

## Security Note

This application requires sensitive information such as API keys and Twilio credentials. Ensure these are kept secure and not exposed publicly. Using environment variables or other secure methods to handle these credentials is recommended.

## Contribution

Contributions, feedback, and suggestions are welcome. Feel free to fork the project, make improvements, or suggest changes.


