# Coinhub_ETL -- Financial Market Data Pipeline
Apis, Web Scrapping


## Project Overview

Coinhub automates the collection of cryptocurrency market data from multiple sources, replacing manual data gathering with a robust ETL pipeline that feeds directly into PostgreSQL for dashboard visualization.

## Business Problem

- **Manual Process**: Analysts manually visiting multiple websites daily
- **Inconsistent Sources**: Data discrepancies across platforms
- **Time-Sensitive**: Crypto markets require real-time updates
- **Human Error**: Manual collection prone to mistakes

## Tech Stack

- **Python**: Core programming language
- **BeautifulSoup**: Static web scraping
- **Selenium**: Dynamic web scraping
- **PostgreSQL**: Data warehouse
- **CoinGecko API**: Cryptocurrency data endpoint

## Data Sources

1. **CoinGecko API** - Free crypto data API
2. **Yahoo Finance** - Cryptocurrency and stock tickers (static/dynamic scraping)
3. **CoinMarketCap** - Real-time crypto updates (static/dynamic scraping)


## Pipeline Architecture

### Extract
- Pull live data from CoinGecko API
- Scrape Yahoo Finance for market data
- Scrape CoinMarketCap for price updates

### Transform
- Clean and standardize field names
- Format currency values
- Standardize timestamps
- Convert to unified schema

### Load
- Store processed data in PostgreSQL

