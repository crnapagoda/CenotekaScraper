# Web Scraping Project

This project is designed to scrape product information from CENOTEKA.RS. It extracts details such as product names, prices, and image URLs from the website and saves the data into a CSV file.

## Features

- Scrapes product names, prices, and image URLs.
- Supports multiple stores and price points for each product.
- Extracts URLs from a sitemap file.
- Saves the scraped data into a CSV file for easy analysis.

## Setup

1. **Clone the repository:**
    ```sh
    git clone https://github.com/crnapagoda/CenotekaScraper
    cd web_scraping_project
    ```

2. **Install dependencies:**
    Make sure you have Python installed. Then, install the required Python packages:
    ```sh
    pip install selenium requests pandas
    ```

3. **Download ChromeDriver:**
    Download the ChromeDriver that matches your Chrome browser version from [here](https://sites.google.com/a/chromium.org/chromedriver/downloads).
    Extract the downloaded file and place it in the `web_scraping_project` directory.

4. **Update ChromeDriver path:**
    Ensure the path to `chromedriver.exe` in `site1_scraper copy 2.py` is correct:
    ```python
    service = Service(r'C:\Users\admin\Desktop\web_scraping_project\chromedriver-win64\chromedriver.exe')
    ```

5. **Place the sitemap file:**
    Ensure the `sitemapcenotekaofficial.xml` file is in the `web_scraping_project` directory.

## Running the Scraper

1. **Run the scraper:**
    Execute the following command to start the scraping process:
    ```sh
    python site1_scraper\ copy\ 2.py
    ```

2. **Output:**
    The scraped data will be saved to `scraped_data.csv` in the `web_scraping_project` directory.

## Notes

- If you want to run the scraper in headless mode, uncomment the following line in `site1_scraper copy 2.py`:
    ```python
    options.add_argument('--headless')
    ```

- Ensure your Chrome browser is up to date to avoid compatibility issues with ChromeDriver.