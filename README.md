# Stock Volatility Prediction

A portfolio project, **in progress**, to build an application that predicts stock volatility. So far the repo holds study notes and early code from the first lessons, not a finished application.

## Planned scope

1. Pull stock data from the Alpha Vantage API.
2. Write Python classes that extract the data and load it into a database.
3. Build a GARCH time-series model to predict volatility.
4. Wrap it in an application with its own API for fetching data, training models and making predictions.

## What is here

| File | Contents |
|---|---|
| `notes.ipynb` | Working notebook with notes and code, organised by lesson |

The notebook covers so far:

- **Lesson 1, getting data from APIs:** URL components (base URL, path, parameters), keeping the API key in a `.env` file rather than in code, a `get_daily` function, and defensive error handling for bad paths and invalid tickers.
- **Lesson 2, test-driven development:** an Alpha Vantage API class, a SQLite-backed SQL repository class (`insert_table`, `read_table`), assert-based tests written before the code, and comparing daily returns for two stocks.

## Running it

You need Python 3, Jupyter, and an [Alpha Vantage API key](https://www.alphavantage.co/support/#api-key). Put the key in a `.env` file (never commit it), then open `notes.ipynb`.
