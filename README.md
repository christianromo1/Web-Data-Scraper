# Web Data Scraper for News Article Collection

A Python-based web scraping framework designed to automatically crawl news websites, extract article content, and generate structured datasets suitable for machine learning and data analysis.

This project was developed as part of a university assignment focused on building automated pipelines for collecting training data from online sources.

---

## Project Overview

This scraper recursively crawls selected news websites, identifies article pages, extracts structured information, and exports the results into a dataset.

The system uses browser automation, HTML parsing, and custom extraction rules to collect:

- Article titles
- Publication dates
- Article content
- Source metadata

The output can be exported as a **CSV dataset** for further analysis or machine learning workflows.

---

## Features

- Recursive news website crawler
- Automated browser scraping using Selenium
- Proxy integration for improved reliability
- Multi-site article parsing with custom selectors
- Content extraction using BeautifulSoup
- Structured dataset export (CSV)
- Debugging and testing utilities
- Optional web interface using Streamlit

---

## Technologies Used

Python  
Selenium WebDriver  
BeautifulSoup  
Streamlit  
Requests  
Regular Expressions  
CSV Data Processing  

---

## Supported News Sources

The scraper includes custom parsing logic for several news websites, including:

- The Federalist
- Daily Wire
- The American Conservative
- The Post Millennial
- Spectator

Each site uses custom HTML selectors to reliably extract article content.

---

## How It Works

### 1. Crawling

The crawler recursively scans web pages to discover article URLs.

The crawler:

- Tracks visited URLs
- Filters links based on article patterns
- limits crawl depth to avoid excessive requests
- introduces randomized delays to mimic human browsing

---

### 2. Scraping

The scraper retrieves full HTML pages using Selenium.

Features include:

- Headless Chrome browser automation
- proxy support for scraping reliability
- dynamic page loading support
- automatic retry logic

---

### 3. Parsing

Extracted HTML is parsed using BeautifulSoup to collect structured data.

The parser extracts:

- title
- publication date
- article content

using custom CSS selectors tailored to each news site.

---

### 4. Data Export

Collected articles are stored as structured records and exported as CSV datasets.

Example output fields:  
title  
date  
content  
leaning  



---

## Running the Project

### Install Dependencies 
bash: pip install selenium beautifulsoup4 streamlit

Run the Scraper: python main.py

---
# Disclaimer

This project was built for educational and research purposes as part of a university coursework assignment.

---
# Author
Christian Romo
Cybersecurity Student
Loyola University Chicago
