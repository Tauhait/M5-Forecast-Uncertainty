# Makridakis-Forecast-Walmart
Estimate the uncertainty distribution of Walmart unit sales.

> https://www.kaggle.com/competitions/m5-forecasting-accuracy  

## About Data
Walmart provided the data. It consisted of 42,840 daily sales time series of items hierarchically
arranged into departments, categories, and stores spread in three U.S. states (the time series are
somewhat correlated with each other). Along with the sales, Walmart also provided accompanying
information (exogenous variables, usually not often provided in forecasting problems) such as
the prices of items, some calendar information, associated promotions, or the presence of other
events affecting the sales. The data represented the USA market: it originated from 10 stores in California, Wisconsin, and Texas. Specifically, the data was made up of the sales of 3,049 products, organized into 3 categories (hobbies, food, and household) that can be divided furthermore into 7 departments each. 

### Hierarchical structure challenge: 
We can model sale dynamics at the level of the USA market, state market, single store, product category, category department, and finally, specific product.

<picture>
 <source media="(prefers-color-scheme: dark)" srcset="imgs/data-hierarchy-m5.png">
 <source media="(prefers-color-scheme: light)" srcset="imgs/data-hierarchy-m5.png">
 <img alt="data hierarchy" src="imgs/data-hierarchy-m5.png">
</picture>

From the point of view of time, the granularity is daily sales record and covered the period spanning from January 29th 2011 to June 19th 2016, which equals to 1,969 days in total: 1,913 for training, 28 for validation (public leaderboard), and 28 for testing (private leaderboard). 
