# Web Scraping Project – Largest U.S. Companies by Revenue

## Overview

This project demonstrates how to perform web scraping using Python to extract tabular data from Wikipedia and store it in a CSV file.

The script scrapes the list of the largest companies in the United States by revenue from Wikipedia, processes the table data using BeautifulSoup and Pandas, and exports the cleaned dataset into a CSV file.



## Project Objective

* Learn the basics of web scraping using Python.
* Extract HTML table data from a website.
* Convert scraped data into a structured Pandas DataFrame.
* Save the extracted data into a CSV file for further analysis.


## Technologies Used

* Python
* BeautifulSoup (`bs4`)
* Requests
* Pandas
* Jupyter Notebook


## Project Structure

```text
├── web scraping.ipynb    # Main Jupyter notebook containing the scraping code
├── Companies.csv         # Output CSV file generated after scraping
└── README.md             # Project documentation
```


## Website Scraped

Data Source:

* Wikipedia – List of Largest Companies in the United States by Revenue



## Features

* Sends HTTP requests to fetch webpage content.
* Parses HTML using BeautifulSoup.
* Extracts table headers and rows dynamically.
* Stores data in a Pandas DataFrame.
* Exports the dataset into CSV format.



## Installation

Install the required libraries before running the project:

```bash
pip install beautifulsoup4 requests pandas
```



## How to Run the Project

1. Clone or download the project.
2. Open the Jupyter Notebook:

```bash
jupyter notebook
```

3. Open:

```text
web scraping.ipynb
```

4. Run all notebook cells.
5. The scraped data will be saved as:

```text
Companies.csv
```



## Sample Workflow

### Step 1: Import Libraries

```python
from bs4 import BeautifulSoup
import requests
import pandas as pd
```

### Step 2: Send Request to Website

```python
url = 'https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue'
page = requests.get(url)
```

### Step 3: Parse HTML Content

```python
soup = BeautifulSoup(page.text, 'html.parser')
```

### Step 4: Extract Table Data

```python
table = soup.find('table', class_='wikitable sortable')
```

### Step 5: Save Data to CSV

```python
df.to_csv('Companies.csv', index=False)
```



## Output

The final output is a CSV file containing company details such as:

* Rank
* Name
* Industry
* Revenue
* Number of Employees
* Headquarters



## Learning Outcomes

Through this project, you will learn:

* Basics of web scraping
* HTML parsing techniques
* Working with tables in BeautifulSoup
* Data cleaning with Pandas
* Exporting datasets to CSV



## Future Improvements

* Add error handling for failed requests.
* Scrape multiple tables or websites.
* Automate scraping using scheduled tasks.
* Store data in a database.
* Build visualizations from the scraped data.



## Author

Created as a beginner-friendly Python web scraping project for learning and practice.
