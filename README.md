# The Anatomy of Box Office Blow-Outs

Overview
---
This project will explore the use of linear regression to predict global box office revenues for movies. The repository consists of three Jupyter Notebooks:
1. **Web Scraping and Cleanup** - The code used to scrape data from IMDb and aggregate it into a useable DataFrame. 
2. **EDA and Feature Engineering** - This notebook examines the data resulting from the first notebook's web scraping, and creates features (typically "dummified" variables) believed to be correlated with the target variable.
3. **Linear Regression Model** - The final notebook verifies that a linear regression model is appropriate to describe the relationships between the independent and dependent variables, and then implements (trains & tests) the model using Scikit-Learn's library.

Data
---
Data is drawn from two main sources: **IMDb Pro** and **The-Numbers.com**. Prior to running the scraping program, a user of these notebooks can enter two parameters to narrow down their data population, as opposed to pulling every movie within the database. These parameters are: 1) the years the movies were released (I selected 2005-2019), and 2) the minimum global box office the movie needs to clear to be included (I chose $5 million). 

BeautifulSoup was used to scrape key features from both sites, and in the case of IMDB Pro, Selenium was used to login, as an account is required to access the data. After pulling in this data, it was aggregated into a Pandas DataFrame and cleansed (e.g. removing sumbols & punctuation, and limiting lists of actors / directors to one name). 

Most features were sourced from IMDB Pro, however The-Numbers was used for budget data, as well as lists of popular actors, directors, and production companies. For budget data specifically, The-Numbers was considered more accurate and complete than the figures provided by IMDB Pro.

Methodology
---
Features were inspected to determine if any transformations were required before modeling. In addition, features were added one-by-one to the linear regression model, with each step involving a check on whether the feature improved the model's R<sup>2</sup>.
