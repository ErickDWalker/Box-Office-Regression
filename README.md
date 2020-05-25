# Box-Office-Prediction
This project will explore the use of linear regression to predict global box office revenues for movies. Data is drawn from two main sources: **IMDb Pro** and **The-Numbers.com**. The repository consists of three Jupyter Notebooks:
1. **Web Scraping and Cleanup** - The code used to scrape data from IMDb (using BeautifulSoup and Selenium) and compile it into a useable DataFrame. 
2. **EDA and Feature Engineering** - This notebook examines the data resulting from the first notebook's web scraping, and creates features (typically "dummified" variables) believed to possess meaningful relationships with the target variable.
3. **Linear Regression Model** - The final notebook verifies that a linear regression model is appropriate to describe the relationships between the independent and dependent variables, and then implements (trains & tests) the model using Scikit-Learn's library.
