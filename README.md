# Exploring-the-World-of-Web-Scraping
Unveiling the Top Grossing Films From Wikipedia

In this project, web scraping techniques were employed using Python libraries BeautifulSoup, Requests, as well as Pandas to collect and analyze the web page and extract the data needed.

Web Scraping: 
This task was completed using BeautifulSoup and Pandas. The process I took is as follows:

Importing Modules/Libraries: I started by importing the necessary libraries and modules, BeautifulSoup for HTML parsing, Requests for making HTTP requests, and Pandas for data manipulation.

Data Source definition: For web scraping in Python, the URL/link of the data source needs to be defined, and for this project the data source was Wikipedia, specifically the page that contained the data of the highest-grossing films till date.

Data Parsing: BeautifulSoup was used to parse the HTML content to extract relevant information, such as review text, movie name, and other details.

Iterative Scraping: There were more than 2 tables on the page, to be definite about which of the tables to extract data from, the .find method which included the table's details (i.e tag and class) was used to point to the exact table needed. The header for the columns was first extracted and populated into the DataFrame. Utilizing a for loop, each film data was located using it's tag and class (just as was done for the headers) in the HTML content, and then it was retrieved.

Data Conversion: The extracted data was converted into a Pandas DataFrame to facilitate further analysis.

Data Saving: Finally, the cleaned data was saved as a CSV file (film_data.csv) for future analysis.

Data Cleaning:
The steps taken to clean the data for analysis as explained below:
Loading Data: The CSV file was read using Pandas, and the DataFrame was labeled "film". The data was then explored using the .dtypes().

Dropping Irrelevant Columns: Columns not required for the analysis were dropped using the .drop method.

Column Cleaning: The Worldwide gross column was saved to the DataFrame as an object and for the purpose of the project it needed to be numeric data. To achieve this first the commas were removed, then specific patterns ($ sign and text) were removed from each record using indexing and slicing. 

