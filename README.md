# Web Scraping Challenge
Estelle Santini | UC Berkeley Data Analytics Bootcamp | 05/11/2023

## Background
This assignment is a full web-scraping and data analysis project where I identified HTML elements, identified their id and class attributes, and used this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. I’ve also learned to scrape various types of information including HTML tables and recurring elements, like multiple news articles on a webpage.

## Deliverables

Deliverable 1: Scrape titles and preview text from Mars news articles.

Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

## Deliverable 1: Scrape Titles and Preview Text from Mars News
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.

Use automated browsing to visit the Mars news siteLinks to an external site. Inspect the page to identify which elements to scrape. Then, extract the titles and preview text of the news articles that you scraped. Store each title-and-preview pair that was scraped in a Python dictionary and, give each dictionary two keys: title and preview. Print the list in your notebook.

## Deliverable 2: Scrape and Analyze Mars Weather Data
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.

Use automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.

Assemble the scraped data into a Pandas DataFrame from the table on the webpage. The columns should have the same headings as the table on the website. Here’s an explanation of the column headings:

**Column Descriptions** 
id: the identification number of a single transmission from the Curiosity rover
terrestrial_date: the date on Earth
sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars
ls: the solar longitude
month: the Martian month
min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)
pressure: The atmospheric pressure at Curiosity's location

Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

**Analysis**

Analyze your dataset by using Pandas functions to answer the following questions:

1. How many months exist on Mars?
2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
3. What are the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question, find the average minimum daily temperature for all of the months. Plot the results as a 4. Which months have the lowest and the highest atmospheric pressure on Mars? To answer this question find the average daily atmospheric pressure of all the months.
Plot the results as a bar chart.
5. About how many terrestrial (Earth) days exist in a Martian year? To answer this question consider how many days elapse on Earth in the time that Mars circles the Sun once.
6. Visually estimate the result by plotting the daily minimum temperature.

Export the DataFrame to a CSV file.