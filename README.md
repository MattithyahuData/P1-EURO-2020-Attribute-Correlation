# ⚽ World Cup 2022 Prediction: Project Overview 
* End to end project reasearching the effects certain attributes have on the value of a car
* Optimized Linear, Lasso, and Random Forest Regressors using GridsearchCV to reach the best model. 
* Built a client facing API using flask 

[View Deployed Model](https://carsalepricecalc.herokuapp.com/)

## Resources Used
**Python 3.8.12, SSIS** 

[**Anaconda Packages:**](requirements.txt) *pip install listed* --  pandas, numpy, scikit-learn
pip install lxml

Kaggle Data source links: [results](https://www.kaggle.com/martj42/international-football-results-from-1872-to-2017/data?select=results.csv) [fifa_rankings](https://www.kaggle.com/tadhgfitzgerald/fifa-international-soccer-mens-ranking-1993now) [fixtures](https://fixturedownload.com/feed/json/fifa-world-cup-2018)
Sources: Kaggle.com, fixturedownload.com


## Data Collection
Source: Kaggle | Webscraping AVG Rupees/GBP conversion data
*	Year	
*   Selling_Price	
*   Present_Price	
*   Kms_Driven	
*   Fuel_Type	
*   Seller_Type	
*   Transmission	
*   Owner
-------
*   Conversion


## Data Cleaning
After I had sraped and downloaded all the data I needed, I needed to clean it up so that it was usable for the model and analysis. I made the following changes and created the following variables:

*	Parsed numeric data out of salary 
*	Made columns for employer provided salary and hourly wages 
*	Removed rows without salary 
*	Parsed rating out of company text 
*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 


## Exploratory data analysis 
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights from the pivot tables. 

![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/salary_by_job_title.PNG "Salary by Position")
![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/positions_by_state.png "Job Opportunities by State")
![alt text](https://github.com/PlayingNumbers/ds_salary_proj/blob/master/correlation_visual.png "Correlations")


## Data Warehousing
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 


## Data Visualisation
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## Data Analytics
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## Business Intelligence
AAAAAAAAAAAAAAAAAAAAAAAAA

*	Made a new column for company state 
*	Added a column for if the job was at the company’s headquarters 
*	Transformed founded date into age of company 

## ML/DL Model Building 

First, I transformed the categorical variables into dummy variables. I also split the data into train and tests sets with a test size of 20%.   

I tried three different models and evaluated them using Mean Absolute Error. I chose MAE because it is relatively easy to interpret and outliers aren’t particularly bad in for this type of model.   

I tried three different models:
*	**Multiple Linear Regression** – Baseline for the model
*	**Lasso Regression** – Because of the sparse data from the many categorical variables, I thought a normalized regression like lasso would be effective.
*	**Random Forest** – Again, with the sparsity associated with the data, I thought that this would be a good fit. 

## Model performance
The Random Forest model far outperformed the other approaches on the test and validation sets. 
*	**Random Forest** : MAE = 11.22
*	**Linear Regression**: MAE = 18.86
*	**Ridge Regression**: MAE = 19.67

## Deployment 
In this step, I built a flask API endpoint that was hosted on a local webserver by following along with the TDS tutorial in the reference section above. The API endpoint takes in a request with a list of values from a job listing and returns an estimated salary. 

## Evaluation 
In this step, I built a flask API endpoint that was hosted on a local webserver by following along with the TDS tutorial in the reference section above. The API endpoint takes in a request with a list of values from a job listing and returns an estimated salary. 


# Data Source Link: 
[]()







DATA SCIENCE 




# Amazon product status checks


READ ME TEMPLATE 
DAT SOURCE DESCP 
DATA SOURE LINK ..... 

What Data did you collect, how often did you collect it? 

## FILE RAN SUCCESSFULLY FOR 3 DAYS.... 
## Project Overview
- We need to know which factors influence to give a loan
- We also need to look for any opportunity to increase the bank's assets.
- It was found that apart from income, family size is an important factor.
- The libraries used were pandas, numpy, matplotlib, seaborn and scipy.
- You can access the Jupiter Notebook at this **[LINK](https://github.com/MattithyahuData/P3-Amazon-Webscraping/blob/master/P3%20Code.ipynb)**

## Objectives
Central question:

**What is the most important factor to give a personal loan?**.

Other questions:
* What is the relationship between education and personal loan?
* What is the distribution of the client population?
* What types of accounts and security do our clients have?
* What is the relationship between income and loans?
* What is the relationship between mortgage and loans?

## Data cleaning and preparation
After importing the libraries we prepared the data for analysis.
- Elimination of negative values and useless columns
- Exploration of the correlation of data and outliers: There is a strong correlation between age and experience

![Heat map of data distribution](Images/Correlation_heatmap.png)

- Analysis of the distribution of the data: A large number of outliers were found in income

![Outliers](Images/Boxplot_outliers.png)

![Histogram](Images/Data distribution.png)

## EDA
The exploratory data analysis was done with the target questions in mind. Several conclusions were obtained which will be presented below.

- Distribution of client education: The most of clients are undergraduates but it appears that education does not have a direct relationship with personal loan.

![Pie Chart: Education Level](Images/Pie_chart_Education.png)

![Personal loan and education](Images/Boxplot_personal_loan.png)

- Analysis of client account type: The vast majority of clients do not have a security or credit account. It could generate some extra assets for the bank if we find a way to encourage them to have one.

![Pie chart, security and credit](Images/Pie_chart_Account_type.png)

- Personal loan in relation to other factors: It seems that the most important factor for a loan is income, no surprise there. Another really important factor is the number of relatives in the family.

![Personal Loan and Income](Images/Income_personal_loan.png)

## Conclusions
- The most influential values are income and family size.
- The least influential values are age and experience. 
- It is advisable to encourage customers to create a credit account and security.
- You can access the code in this **[LINK](https://github.com/Roberto121c/Bank_loans_analysis/blob/main/Code/Finance_data_analysis.ipynb)**



* Goal: Web scrape data to find a if there is a correlation between team attributes and team rank in The UEFA European Championship.


*Based on Euro 2020 data


* Conclusion: The higher the average market value and the younger the average age of a team the higher they will rank. 

* BI Options for action:
1. Select players with the highest market values.
2. Select more younger players. 

Project Managment
2 week Sprint 
- Jira
- Confluence
- Trello 

#### To see more projects CLICK [here](https://mattithyahudata.github.io/devportfolio/).
##### If you have any questions on the project [EMAIL ME](mailto:mattithyahuowolabi@gmail.com) 