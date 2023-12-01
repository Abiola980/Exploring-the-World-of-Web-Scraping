# Exploring-the-World-of-Web-Scraping
Unveiling the Top Grossing Films From Wikipedia

In this project, web scraping techniques were employed using Python libraries BeautifulSoup, Requests, as well as Pandas to collect and analyze the web page and extract the data needed.

Web Scraping with BeautifulSoup and Pandas The process can be broken down into the following steps:
Importing Libraries: I started by importing the necessary libraries and modules, BeautifulSoup for HTML parsing, Requests for making HTTP requests, and Pandas for data manipulation.
Defining the Data Source: The data source was Wikipedia, specifically the page that contained the data of the top-grossing films till date.
Data Parsing: BeautifulSoup was used to parse the HTML content to extract relevant information, such as review text, movie name, and other details.
Iterative Scraping: There were more than 2 tables on the page, utilizing a for loop, each film data was located using it's tag and class in the HTML content, and then it was retrieved.
Data Conversion: The extracted data was converted into a Pandas DataFrame to facilitate further analysis.
Data Saving: Finally, the cleaned data was saved as a CSV file (film_data.csv) for future analysis.

