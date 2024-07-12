# Estimating Market-Implied Probability of Default for Corporate Bonds

This project estimates the market-implied probability of default (PD) for corporate bonds using data scraping, data cleaning, and financial analysis techniques.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Workflow](#workflow)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The goal of this project is to estimate the probability of default for corporate bonds based on market data. The project involves scraping bond data, cleaning and transforming the data, estimating the risk-adjusted discount rate, calculating the market-implied probability of default, and comparing it with ratings-implied PDs.

## Installation

To install the required packages, run the following commands:

```bash
!playwright install
!pip install playwright
!pip install pandas
!pip install yfinance
!pip install matplotlib
!pip install beautifulsoup4
```

## Usage

1. **Data Collection**: Use Playwright to scrape bond data from the FINRA website.
2. **Data Cleaning and Transformation**: Clean and transform the scraped data using Pandas.
3. **Estimating Risk-Adjusted Discount Rate**: Calculate the market rate of return using the risk-free rate and market risk premium.
4. **Estimating Market-Implied Probability of Default**: Calculate the probability of default using a custom function.
5. **Comparing PDs with Ratings-Implied PDs**: Compare the market-implied PDs with ratings-implied PDs using data from a rating transition study.

## Workflow

Here is a high-level overview of the workflow:

1. **Data Collection**:
    - Install dependencies
    - Scrape bond data
2. **Data Cleaning and Transformation**:
    - Convert data types
    - Drop rows with missing values
    - Calculate maturity years
    - Filter bonds with maturity up to 5 years
3. **Estimating Risk-Adjusted Discount Rate**:
    - Fetch risk-free rate
    - Define market risk premium
    - Calculate market rate of return
4. **Estimating Market-Implied Probability of Default**:
    - Define the `bonds_probability_of_default` function
    - Estimate PD for each bond
5. **Comparing PDs with Ratings-Implied PDs**:
    - Load and clean rating transition data
    - Map ratings to standardized values
    - Plot the results

## Dependencies

- `playwright`: For web scraping.
- `pandas`: For data manipulation.
- `yfinance`: For fetching financial data.
- `matplotlib`: For plotting data.
- `beautifulsoup4`: For parsing HTML.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
