# Project: IPO Scraper

## Project Overview

This project consists of a Python script, `ipo_scraper.py`, designed to scrape Initial Public Offering (IPO) data from `ipowatch.in`. It gathers information on IPO subscriptions and Grey Market Premium (GMP), cleans and processes the data using the `pandas` library, and then merges the two datasets. The final, consolidated data is saved to a JSON file named `merged_ipo_data.json`.

The core technologies used in this script are:
- **Python:** The scripting language.
- **requests:** For making HTTP requests to fetch the web pages.
- **BeautifulSoup:** For parsing the HTML content.
- **pandas:** For data manipulation and analysis.
- **numpy:** For numerical operations.

## Building and Running

### Prerequisites

To run this script, you need to have Python installed, along with the necessary libraries. You can install the dependencies using pip:

```bash
pip install requests beautifulsoup4 pandas numpy
```

### Execution

To execute the script and generate the `merged_ipo_data.json` file, run the following command in your terminal:

```bash
python ipo_scraper.py
```

The script will print its progress to the console and, upon successful completion, will create the `merged_ipo_data.json` file in the same directory.

## Development Conventions

The script is self-contained within `ipo_scraper.py`. The logic is organized into several functions:

- `fetch_and_parse_table`: A generic function to fetch and parse HTML tables from a URL.
- `normalize_stock_name`: A utility function to clean and standardize IPO names.
- `clean_numeric_column`: A function to clean and convert data columns to a numeric type.
- `main`: The main function that orchestrates the scraping, processing, and saving of the data.

The script follows a clear, linear flow within the `main` function:
1.  Fetch subscription data.
2.  Fetch GMP data.
3.  Normalize and clean the data in each DataFrame.
4.  Merge the two DataFrames.
5.  Filter out incomplete records.
6.  Print the final data to the console.
7.  Save the merged data to a JSON file.
