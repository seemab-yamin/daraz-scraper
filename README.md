# Daraz Product Scraper
Daraz product scraper is a powerful Python scraper, built with Scrapy and Playwright, conquers Daraz's dynamic content and anti-bot measures. It extracts product details (titles, prices, etc.) while respecting robots.txt and handles complex product structures. It even cleans and converts prices to USD!

## Goal:
- Handle Dynamic Content rendering in a headless mode.
- Handle anti-bot services to bypass blocking
- Respects robots.txt guidelines
- Extracting Complex Product Listing Structure and Extract Dynamic Prices
- Implemented Data Validation like cleaning prices data and converting into Dollars($)
- Navigates to next page until reaches last page and handle pagination
- Implemented Download Delay to avoid server overloading.

## OS Platform:

Python 3 (Linux/Mac/WSL)

## Installing Dependencies:

To install dependencies open terminal and type:

```Bash
git clone https://github.com/seemab-yamin/daraz-product-scraper
cd daraz-product-scraper
pip install -r requirements.txt
playwright install --with-deps chromium
```

Run:
```Bash
python3 scraper.py {category_url}

# Example
python3 scraper.py https://www.daraz.pk/vented-dryers
```

## Pros: 
- Store Details logs for later debugging
- Can increase CONCURRENT_REQUESTS to initiate more instances to speed up things but will consume more resources.

## Cons:
- Browser based solutions are Memory expensive so should be used in specific use cases like: Bypass blocking, Load Dynamic Content, Perform Automation, etc

## Improvements:
- Need to add explicit time sleep or scroll as Images weren't fully rendered in the page source.

# Dataset Screenshot:
![Dataset Image](daraz_products_dataset.PNG)

# Video Demo:
[![Demo Video](https://i.ytimg.com/vi/qLcY0ZkxuN8/sddefault.jpg?sqp=-oaymwEmCIAFEOAD8quKqQMa8AEB-AHWBIAC4AOKAgwIABABGCQgWyh_MA8=&rs=AOn4CLAgXfCHzvKbSuHq33QxKO7L2Qdq2w)](https://youtu.be/qLcY0ZkxuN8)

## Resources:

- Scrapy: https://scrapy.org/
- Scrapy-Playwright: https://github.com/scrapy-plugins/scrapy-playwright
- Scrapy-Playwright Tutorial: https://scrapeops.io/python-scrapy-playbook/scrapy-playwright/