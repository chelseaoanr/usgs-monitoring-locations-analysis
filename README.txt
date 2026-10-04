# USGS Monitoring Locations Web Scraping & Analysis

This project uses Python and BeautifulSoup to scrape monitoring-location data from the U.S. Geological Survey Water Data API. The project collects 50,000 monitoring-location records across 25 paginated pages, cleans the scraped data, and performs descriptive statistical analysis.

## Tools Used

- Python
- BeautifulSoup
- Requests
- Pandas
- Jupyter Notebook

## Project Workflow

- Scraped 25 pages of USGS monitoring-location data
- Collected 50,000 records using cursor-based pagination
- Converted scraped HTML tables into a Pandas DataFrame
- Identified and handled missing values
- Checked for duplicate records
- Converted altitude variables to numeric data
- Analyzed monitoring-location frequency by state
- Compared altitude distributions by state
- Calculated altitude range, standard deviation, variance, and IQR
- Evaluated average altitude measurement accuracy

## Key Findings

- Arkansas represented 99.39% of the 50,000 scraped monitoring-location records.
- Arkansas had 12,379 valid altitude measurements.
- Mean altitude was approximately 206.88, with a median of 204.
- The middle 50% of altitude measurements fell within a 33-unit range.
- Arkansas had an average altitude measurement error of approximately 1.81.

## Data Source

USGS Water Data API. The dataset was collected directly from the USGS monitoring-locations website using Python, Requests, and BeautifulSoup. A pre-existing CSV file was not used.