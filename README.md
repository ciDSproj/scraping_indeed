# Indeed Jobs Web Scraping and Analysis: Project Overview
-	Scraped over 1200 job descriptions from Indeed web pages
-	Visualized the companies and the locations with the highest number of job listings
-	Calculated the average minim and maxim salary 
-	Engineered features from the text of each job description to quantify the value companies put on specific tools, platforms, skills, and data science roles
-	Created a word cloud highlighting the most frequently used words in job descriptions

## Code and Resources Used
- Python 3.7
- Requests library and Beautiful Soup module for reading the HTML content and convert it to a readable format
- NumPy and Pandas libraries for data manipulation
- Matplotlib and Seaborn for visualizations
- Natural Language Toolkit (NLTK) for text analysis

## Web Scraping
I scraped more than 1200 data science jobs from Indeed.com. This involved the following steps:
- define function to access the HTML content from the webpage
- define function for searching and extracting all details for a job posting
- save the results to a csv file
- repeat the steps above using different search criteria
- merge all data into a final csv file

With each job I got the following data:
- Job Title
- Salary
- Job Description
- Company
- Location

## Data Cleaning
After scraping the data, I needed to clean it up so it can be used for analysis. I made the following changes and created new variables:
-	Remove duplicates
-	Group the jobs by Company and by Location
-	Calculate the average minim and maxim salary:
     -	drop the rows with missing values for salary and reset index
     -	check the formatting of the salary column
     -	define a function to format, calculate, and split salary in minim and maxim values
     -	create two new columns with minim and maxim salary for each job 
     -	determine the mean values of the columns with minim and maxim salary
-	Text cleaning and preparation
    -	define a function to clean the text: tokenize, convert to lowercase, replace special characters, filter the stopwords
    -	create a dictionary with each word and the sum of its occurrences in the text
    -	make a dataframe with unique words and the count for each of them
-	Create a Word Cloud using the most frequent words in job descriptions

## EDA
Using data analysis and visualizations, I tried to find answers to some questions: 
-	Which companies or locations have the highest number of job listings?
-	What is the average minim and maxim salary?
-	What is the frequency of words for specific tools and platforms, skills, and roles?
-	Which are the most frequent words in job descriptions and job titles?
