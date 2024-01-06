
# Flipkart iPhone Scraping Project

## Overview

This project involves web scraping data from Flipkart to gather information about various iPhone products, including details like product names, prices, ratings, storage capacities, sizes, camera specifications, and processors. The data is collected from multiple pages on the Flipkart website using the BeautifulSoup library for parsing HTML and the requests library for making HTTP requests. The scraped data is then stored in a Pandas DataFrame and exported to a CSV file for further analysis or use.

## Prerequisites

To run this project, you need to have the following libraries installed:

-   bs4 (BeautifulSoup)
-   pandas
-   requests

You can install these libraries using the following commands:

```bash
pip install beautifulsoup4
pip install pandas
pip install requests` 
```

## Project Structure

The project consists of two main parts:

1.  **Single Page Scraping (Jupyter Notebook Cell 1-44):**
    
    -   The initial code demonstrates how to scrape data from a single page on Flipkart.
    -   It extracts information for a single product, including product name, price, rating, storage, size, camera specifications, and processor.
    -   The data is then stored in lists and converted into a Pandas DataFrame.
2.  **Multi-Page Scraping (Jupyter Notebook Cell 45-65):**
    
    -   A function `scrape_page` is defined to scrape data from a given page URL.
    -   A loop is used to iterate over multiple pages, calling the `scrape_page` function for each page.
    -   The scraped data from each page is appended to the DataFrame created for the first page.
3.  **CSV Export (Jupyter Notebook Cell 66-69):**
    
    -   The final DataFrame is converted to a CSV file named 'products.csv'.
    -   The CSV file serves as a structured data representation of the scraped information.

## How to Run

1.  Open the Jupyter Notebook in your preferred environment.
2.  Run each cell in order, ensuring all libraries are installed.
3.  Check the 'products.csv' file in the same directory for the exported data.

## Note

-   Ensure that you are compliant with Flipkart's terms of service when scraping data from their website.
-   The number of pages to scrape is customizable by modifying the `total_pages` variable.
