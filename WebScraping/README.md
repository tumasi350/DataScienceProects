# Yelp Restaurant Web Scraper

## Project Overview

Developed a web scraper to gather information about restaurants in Chicago and Oak Park from Yelp. The scraper collects data on the number of reviews, ratings, types of cuisine, and comments. The project utilizes BeautifulSoup for web scraping and pandas for data processing.
This code is WIP.

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools and Libraries](#tools-and-libraries)
- [Web Scraping Process](#web-scraping-process)
- [Data Storage](#data-storage)
- [Results/Findings](#resultsfindings)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [References](#references)

## Data Sources

- Yelp website: Contains information about restaurants, including reviews, ratings, and other details.

## Tools and Libraries

- **Python Version:** 3.9
- **Libraries:** 
  - `requests`
  - `beautifulsoup4`
  - `pandas`

## Web Scraping Process

The web scraping process involved the following steps:
1. **Data loading and inspection**: Sending HTTP requests to Yelp and parsing the HTML content.
2. **Extraction of restaurant details**: Extracting restaurant names, URLs, ratings, and review counts.
3. **Iterating through multiple pages**: Handling pagination to scrape data from multiple pages.

## Data Storage

The extracted data is stored in a pandas DataFrame, which is then exported to a CSV file for further analysis.

## Results/Findings

The scraper successfully collected data on numerous restaurants in Chicago and Oak Park. The dataset includes restaurant names, URLs, ratings, review counts, and types of cuisine.

## Recommendations

Based on the scraping process and initial analysis, the following actions are recommended:
- **Data Cleaning**: Clean and preprocess the scraped data to handle missing values and inconsistencies.
- **Data Analysis**: Perform detailed data analysis to gain insights into restaurant ratings, review patterns, and popular cuisines.
- **Automation**: Schedule the scraper to run at regular intervals to keep the dataset updated.

## Limitations

The scraper relies on the current structure of Yelp's website, and any changes to the website's HTML structure may require updates to the scraper code. Additionally, the scraper may be limited by Yelp's rate limiting and anti-scraping measures.

## References

1. [BeautifulSoup Documentation](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
2. [Requests Documentation](https://docs.python-requests.org/en/master/)
3. [Pandas Documentation](https://pandas.pydata.org/)
4. [Shreyah Singh Medium](https://shreya-singh1.medium.com/building-an-end-to-end-yelp-scrapper-using-python-and-beautiful-soup-ee4c2bcfca9b)

