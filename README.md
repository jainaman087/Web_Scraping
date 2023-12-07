# Building a News Aggregation Pipeline


## Overview

This Jupyter Notebook is designed to scrape the top 100 news items for each of the specified categories (technology, automobile, science, and hatke) from the "inshorts" news platform. 
The extracted information includes Date, Time, Author, Title, Body, Published Source, and Category for each news item. The data is then stored in a SQLite database, and a word cloud visualization is generated based on the frequency of selected keywords.





## Installation

- Python 3.x
- BeautifulSoup
- Requests
- json
- pandas
- sqlite3
- wordcloud
- matplotlib
## File Structure

Inshorts_Assignment.ipynb: Main Python script for news scraping, database creation, and keyword analysis.

### Explanation of Python Scripts-

### Table of Sections-
### Section 1- Data Retrieval:

Fetch the top 100 news items for each category: Technology, Automobile, Science, and Hatke from the "inshorts" news platform.
Extract the following information for each news item: Date, Time, Author, Title, Body,Published Source, Category.

#### Explanation:

The provided section performs web scraping on the Inshorts news website to extract information from trending topics in specified categories such as Technology, Automobile, Science, and Hatke. It uses a loop to iterate through pages and categories, making API requests to retrieve news data. The extracted information includes the publication date and time, author name, news title, content, source name, and category for each news item. Finally, the data is organized into a Pandas DataFrame for further analysis or storage.

### Section 2- Data Storage:

Design a relational database schema to store the extracted information.
Pipeline the data into the designed database.

#### Database Information:
The SQLite database file is named news_database.db.
The News_Items table contains the following columns: S_No, Date, Time, Author, Title, Body, Published_Source, Category.
Word Cloud Visualization:

### Section 3- Keyword Analysis:

Create a word cloud visualization based on the frequency of the following keywords in the fetched articles: "Diwali", "Offer", "Discount", "Dhamaka", "Dead", "Fire", "Burn".

#### Explanation:
The provided section generates a word cloud using the WordCloud library and matplotlib. It focuses on specific keywords related to Diwali, such as "Diwali," "Offer," "Discount," "Dhamaka," "Dead," "Fire," and "Burn." The code combines text from the 'Title' and 'Body' columns of a DataFrame into a single column named 'Text.' It then counts the frequency of each keyword in the combined text and creates a word cloud visualizing the keywords based on their respective frequencies. The resulting word cloud is displayed using matplotlib.



## Usage
- Open and run the Inshorts_Assignment.ipynb Jupyter Notebook to execute the web scraping, data processing, and keyword analysis.

- The scraped news data is stored in the news_database.db SQLite database. You can query this database or use it for further analysis.

- Explore the word cloud visualization in the notebook to understand the frequency of specified keywords in the news articles.



