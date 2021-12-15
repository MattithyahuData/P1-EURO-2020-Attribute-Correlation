# ⚽ World Cup 2018 Prediction: Project Overview 
* End to end project reasearching the effects certain attributes have on the value of a car
* Optimized Linear Regression model using only relevent data in a date range

[View Code](Code/P1 Code.ipynb)

## Resources Used
**Python 3.8.12** 

[**Anaconda Packages:**](requirements.txt) **pandas, numpy, scikit-learn**

Kaggle Data source links: 
* [results](https://www.kaggle.com/martj42/international-football-results-from-1872-to-2017/data?select=results.csv) 
* [fifa_rankings](https://www.kaggle.com/tadhgfitzgerald/fifa-international-soccer-mens-ranking-1993now) 
* [fixtures](https://fixturedownload.com/feed/json/fifa-world-cup-2018)


## Data Collection
Download Sources: Kaggle | fixturedownload
* Using all international game data was key, as we needed past instances of teams performances
* Here I downloaded the datasources from Kaggle as a csv
* I used the read_json function to read the fixtures data into python


## Data processes
Mainly an optimisation project to see if shortening the years of data used would maybe imporve the model performance.

## Evaluation 
Based on the actual results the model did not perform well, in future collecting better quaility data would help witht hw quality of the model and the prediciton. 
Also not every think requires machine learning! Know when to and when not to use it. 


## Conclusions
* Filtering out irrelevant historic match data

The highest level of football before Senior football is U21 football. For national teams the AVG squad age is between 24 - 29.6 years. Players under the age of 21 rarely get recruited to the senior team so to accomodated for those that may 21 years old will be our lower bound. To accomodate for older players our upper bound will be 30 years. 

* It is rare for teams to stay together for longer than 5 years in any sport, some people get better in their game and stay others get worse and are dropped, some retire, some leave through injury. The list is endless, based on this number I will only collect data from up to 5 years before the day before the first game of the World Cup

* Because we want a clear view of the performance of the current squad and not the England team of 1966 for example because that isnt the team playing now. A limit of 9 years would help imrpove this bias.  
* Currently doing more research to validate any lower or higher number. I will simply update the function input when I get this infor. 
* Past performance of previous squads does not guarantee future performance 

Project Managment (Agile - Scrum)
* Resources used
    * Jira
    * Confluence
    * Trello 


#### To see more projects CLICK [here](https://mattithyahutech.co.uk/).
##### If you have any questions on the project [EMAIL ME](mailto:theanalyticsolutions@gmail.com) 