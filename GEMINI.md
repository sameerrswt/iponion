# Iponion Project

## Project Overview

This project is a full-stack application consisting of a Python-based web scraper for Initial Public Offering (IPO) data and a static HTML/CSS frontend for a consultancy website named "Iponion".

The project is organized into two main directories:

-   `Backend/`: Contains the Python script for scraping IPO data.
-   `Frontend/`: Contains the static website files.

### Backend

The backend is a Python script (`ipo_scraper.py`) that scrapes IPO subscription and Grey Market Premium (GMP) data from `ipowatch.in`. It uses `requests`, `BeautifulSoup`, and `pandas` to fetch, parse, and clean the data. The final merged data is saved as `merged_ipo_data.json`.

For more details, see the `Backend/GEMINI.md` file.

### Frontend

The frontend is a simple, static website for a consultancy named "Iponion". It is built with plain HTML and CSS.

For more details, see the `Frontend/GEMINI.md` file.

## Usage

### Backend

To run the backend script and generate the IPO data file:

1.  **Install dependencies:**
    ```bash
    pip install requests beautifulsoup4 pandas numpy
    ```
2.  **Run the script:**
    ```bash
    python Backend/ipo_scraper.py
    ```

### Frontend

To view the website, open the `Frontend/Index.html` file in a web browser.
