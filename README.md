# beautifulsoup-challenge

## Overview
This project involves web scraping and data analysis of Mars-related information. Using Python tools such as Splinter and Beautiful Soup, data is extracted and processed from two primary sources: Mars news articles and Mars weather data.

## Features

### Part 1: Scrape Titles and Preview Text from Mars News
#### Objective
Scrape the latest Mars news articles to extract their titles and preview text.

#### Key Steps
- **Automated Browsing**: Use Splinter to navigate to the Mars News site and extract HTML code.
- **Data Extraction**: Create a Beautiful Soup object to parse HTML and scrape the titles and preview text of articles.
- **Data Organization**:
  - Store each title and preview text pair in a Python dictionary with the keys `title` and `preview`.
  - Append all dictionaries to a list.


### Part 2: Scrape and Analyze Mars Weather Data
#### Objective
Scrape Mars weather data from an HTML table, analyze it, and visualize key insights.

#### Key Steps
1. **Automated Browsing**: Use Splinter to visit the Mars Temperature Data site and extract the table.
2. **Data Extraction**:
   - Create a Beautiful Soup object to scrape data from the HTML table.
   - Assemble the data into a Pandas DataFrame.
   - Ensure columns have appropriate headings and data types.
3. **Data Analysis**:
   - Determine the number of months on Mars and the total number of Martian days in the dataset.
   - Calculate average minimum daily temperature for each month and visualize results in a bar chart.
   - Calculate average daily atmospheric pressure for each month and visualize results in a bar chart.
   - Estimate the number of Earth days in a Martian year by analyzing temperature trends.
4. **Data Export**: Save the DataFrame to a CSV file.

## Deliverables
- **Jupyter Notebook 1**: Mars News scraping (`part_1_mars_news.ipynb`).
- **Jupyter Notebook 2**: Mars Weather data scraping and analysis (`part_2_mars_weather.ipynb`).
- **Exported CSV File**: Cleaned Mars weather data.

## Setup and Dependencies
Before starting, ensure you have the following libraries installed:

```python
# Dependencies
from splinter import Browser
from bs4 import BeautifulSoup
import matplotlib.pyplot as plt
import pandas as pd
import json
```

## Running the Analysis
- Clone the repository and navigate to the project directory.
- Install dependencies as shown above.
- Run the Jupyter Notebooks to generate the analyses and visualizations.

