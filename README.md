# Indeed Jobs Web Scraping and Analysis: Project Overview
-	Scraped over 1000 job descriptions from Indeed web pages
-	Visualized the companies and the locations with the highest number of job listings
-	Calculated the average minim and maxim salary 
-	Engineered features from the text of each job description to quantify the value companies put on specific tools, platforms, skills, and data science roles
-	Created a word cloud highlighting the most frequently used words in job descriptions

## Code and Resources Used
- Python 3.7
- Requests library for reading the HTML content of the web page
- Beautiful Soup module to convert the content to a readable format
- NumPy and Pandas libraries for data manipulation
- Matplotlib and Seaborn for visualizations
- Natural Language Toolkit (NLTK) for text analysis

## Web Scraping
Scraping the Indeed webpage involved mainly the following steps:
- access the HTML content from the webpage
- search and extract the job details
- save the results to a csv file
- repeat the steps above using different search criteria
- merge all data into a final csv file

I scraped more than 1200 jobs, for each job the following data:
- Job Title
- Salary
- Job Description
- Company
- Location

## Data Cleaning
