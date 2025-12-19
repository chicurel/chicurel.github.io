---
title: 'BOE Scraper'
summary: 'A web scraper written in R for extracting and processing content from the Boletín Oficial del Estado (BOE), the official gazette of Spain, as well as the historical BOE archives ("Gazeta").'
authors:
  - 2025
date: '2025-02-01T00:00:00Z'

tags:
  - Web Scraping
  - Data Analysis
  - Data Visualization
  - Mahcine Learning



url_project: 'https://github.com/chicurel/BOE-Gazeta-Scrapers'
url_pdf: ''
url_dataset: ''
url_slides: ''
url_video: ''

---

# BOE Scraper

A web scraper written in **R** for extracting and processing content from the [Boletín Oficial del Estado (BOE)](https://www.boe.es/), the official gazette of Spain, as well as the **historical BOE archives** ("Gazeta").

## Features

- Extracts metadata (title, date, references, document links) from BOE search result pages
- Downloads linked **PDF**, **XML**, and **HTML** files
- Outputs metadata to structured CSV
- Two scraper modules included:
  - **BOE Scraper (1960–Present)** — from the official digital BOE
  - **Gazette Historical Scraper** — for older historical BOE archives

## How It Works

1. Go to the [BOE website](https://www.boe.es/)
2. Use the search tool to filter by keyword, date range, or section
3. Copy the resulting URL from the browser's address bar
4. Run the appropriate scraper in R, passing the copied URL as input
5. The scraper will:
   - Load all matching publications
   - Extract metadata (title, publication date, section, file links, etc.)
   - Save the data into a structured CSV file

## Scrapers

### 1. BOE Scraper (1960–Present)
### 2. Gazette Historical Scraper (Pre-1960)


## Requirements
- You must create the following folder structure in your working directory:
  - output
  - files
    
- Required R packages:
  - `xml2`
  - `httr`
  - `purrr`
  - `rvest`
  - `curl`
  - `tidyverse`
  - `janitor`
 

Install dependencies with:

```r
install.packages(c("xml2", "httr", "purrr", "rvest", "curl", "tidyverse","janitor"))

