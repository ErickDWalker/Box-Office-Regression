# Box-Office-Prediction
This program will explore the use of linear regression to predict global box office revenues for movies. The repository consists of three notebooks:
1. **Web Scraping and Cleanup** - The code used to extract data from IMDB and convert it into a useable DataFrame. 
2. **EDA and Feature Engineering** - This notebook examines the data resulting from the first notebook's web scraping, and creates features (typically "dummified" variables) believed to possess meaningful relationships with the target variable.
3. **Linear Regression Model** - The final notebook verifies that a linear regression model is appropriate to describe the relationships between the independent and dependent variables, and then implements (train & tests) the model using Scikit-Learn's library.
