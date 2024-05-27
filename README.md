# Mars News and Weather Data Analysis

Background
This project focused on web-scraping and data analysis, utilizing tools such as Splinter for automated browsing and Beautiful Soup for HTML parsing. The goal was to extract, analyze, and visually communicate insights from Mars news articles and weather data.

Deliverables
This project consisted of two main tasks:

Scraping titles and preview text from Mars news articles.
Scraping and analyzing Mars weather data.

Part 1: Scrape Titles and Preview Text from Mars News
Setup: The Jupyter Notebook named part_1_mars_news.ipynb was used.
Automated Browsing: Splinter was used to visit the Mars news site and inspect the page for elements to scrape.
Extract Text Elements:
A Beautiful Soup object was created to parse the HTML.
The titles and preview texts of news articles were extracted.
Each title and preview text was stored in a dictionary with two keys: title and preview.
All dictionaries were stored in a list and printed.
Optionally, the scraped data was exported to a JSON file for easier sharing.

Part 2: Scrape and Analyze Mars Weather Data
Setup: The Jupyter Notebook named part_2_mars_weather.ipynb was used.
Automated Browsing: Splinter was used to visit the Mars Temperature Data Site at Mars Temperature Data Site.
Scrape Data:
A Beautiful Soup object was created to parse the HTML table.
Data was extracted and assembled into a Pandas DataFrame with columns matching the table on the website.
Column Explanation:
id: Identification number of a transmission from the Curiosity rover.
terrestrial_date: Date on Earth.
sol: Number of elapsed sols (Martian days) since Curiosity landed.
ls: Solar longitude.
month: Martian month.
min_temp: Minimum temperature in Celsius of a sol.
pressure: Atmospheric pressure at Curiosity's location.
Data Type Conversion: Columns were converted to appropriate data types (datetime, int, float).

Data Analysis:

The number of months on Mars was determined.
The number of Martian days in the dataset was calculated.
The coldest and warmest months were identified based on average minimum daily temperatures and plotted as a bar chart.
The months with the lowest and highest atmospheric pressures were identified and plotted as a bar chart.
The number of Earth days in a Martian year was estimated by analyzing the temperature data and plotting it.
Export Data: The DataFrame was saved to a CSV file.
