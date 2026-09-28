# Automated Web Scraping: Business Listings

Python pipeline built during my data support internship at Noir Labs to extract business listing details from a website that loads content through infinite scroll.

## What it does
- Selenium scrolls each category page until no new listings load
- BeautifulSoup collects listing links and parses each page
- Extracts name, address, phone number and website into structured columns
- Handles HTTP errors and missing page elements
- Exports one CSV per category (food and drink, home and design, style and beauty, health and wellness, history and culture) plus a combined, de-duplicated file

## Tech
Python, Selenium, BeautifulSoup, urllib, pandas

## Run
pip install selenium beautifulsoup4 pandas
python scrape_business_listings.py
Requires Google Chrome. Output is saved to the `output` folder.
