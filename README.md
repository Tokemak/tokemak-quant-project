# Tokemak Quant Project

The goal of this project is analyze Curve AMM pool & Mav AMM pool using on-chain data. 
  1. Identify various sources of return for an LP 
  2. Recommend which pool is expected to have the best risk-adjusted return for a relatively passive investment strategy. 

## Project Requirements
* use primarily on-chain data. Show code on how the data was pulled and analyzed
* 1-2 pager explaining your thoughts, observation & conclusion

## Example Metrics (Non-Exhaustive)
1. historical total return
2. historical fee return
3. historical volume/turnover/TVL/etc
4. token price volatility

## Project Setup

### Web3 Provider

The project requires an eth node provider for data collection. A public Alchemy URL is in the `example.py` file, but is likely to be rate limited. We recommend getting your own key and adding it to the .env file as `PROVIDER_URL`.

### Dependency Management

The project uses [Poetry](https://python-poetry.org/) as its dependency manager. Below are the steps to get started:

1. install [Poetry](https://python-poetry.org/docs/#installation)
2. run `poetry install` in the root of the project
3. run `poetry run example` (it may be rate limited if you did not add a PROVIDER_URL)
