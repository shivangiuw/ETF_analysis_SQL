# Analysis of Fintech ETF performance 
(Using SQL, Python, and the Voilà library)

* Analyze the daily returns of the ETF stocks both individually and as a whole portfolio through following steps:

1. Analyze the performance of a single asset from the ETF using SQL queries with Python, Pandas, and hvPlot.
2. Build the entire ETF portfolio (using SQL inner join) and read the SQL query as a dataframe. Further evaluate its performance using daily returns, annualized returns and cumulative returns.
3. Visualize the results using interactive hvplots to explore daily returns and cumulative returns.


## Technologies

* [pandas] (https://pandas.pydata.org/docs/getting_started/index.html)- for data analysis

* [jupyter lab] (https://jupyterlab.readthedocs.io/en/stable/)- to work with notebooks, code, data and plots

* [hvplot] (https://hvplot.holoviz.org/user_guide/Introduction.html)- to display an interactively explorable plot with panning, zooming, hovering, and clickable/selectable legends

* [sqlalchemy] (https://www.sqlalchemy.org/)- to facilitate the communication between Python program and databases

* [datetime] (https://docs.python.org/3/library/datetime.html)- to manipulate the datetime format

## Installation Guide

```
 conda install pandas
 pip install jupyterlab
 conda install -c pyviz hvplot geoviews
 
```

## Usage

* The notebook can be used to complete analysis of a fintech ETF that consists of different stocks. Here analysis is done for the four stocks: GOST, GS, PYPL, and SQ. Each stock has its own table in the etf.db database.

* The data for the individual stocks containing time, opening prices, closing prices, daily returns etc. can be pulled from different tables in database through SQL queries and  can be converted to the dataframes.

* Further data for the ETF portfolio can be pulled together from all the stock tables using SQL inner join on the “time” column in SQL query, to join all the tables together and read the query as a dataframe.

* Various analysis tools like calculating average daily returns,annualized returns and cumulative returns can be used for analysis of the portfolio dataframes and results can be plotted using interactive hvplots to visualize the trend.

 
## Contributor

Shivangi Gupta