# Tokemak Quant Project

The goal of this project is analyze Uniswap V2 and SushiSwap AMM pools using on-chain data and recommend 10 pools that are expected to have the best risk-adjusted return for a relatively passive investment strategy.

## Project Requirements

* `data/uni_v2_sushi_pools.csv` has a list of most known pools. This can be considered a definitive list for this project
* only analyze pools where ETH (WETH) are one of the tokens
* use primarily on-chain data. If you have other data sources feel fee to use them, but the project needs to be runnable without additional creds

## Example Metrics (Non-Exhaustive)
1. historical total return
2. historical fee return
3. historical volume/turnover/TVL/etc
4. token price volatility

## Minimum Output

1. A table with stats/metrics used to identify the target pools
2. A summary table with the selected pools
3. A write-up explaining why the pools were selected (can be brief 1-2 paragraphs)
4. [Optional] Other stats/metrics you would look at with more time


## Project Setup

### Web3 Provider

The project requires an eth node provider for data collection. A public Alchemy URL is in the `example.py` file, but is likely to be rate limited. We recommend getting your own key and adding it to the .env file as `PROVIDER_URL`.

### Dependency Management

The project uses [Poetry](https://python-poetry.org/) as its dependency manager. Below are the steps to get started:

1. install [Poetry](https://python-poetry.org/docs/#installation)
2. run `poetry install` in the root of the project
3. run `poetry run example` (it may be rate limited if you did not add a PROVIDER_URL)