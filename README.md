# Module_7_Repo
In this project I created a web application for an ETF Alalyzer. I started by analyzing a single asset in the ETF. I did this by creating a temporary SQLite and using an engine to interact with it. I then created a query in the SQL to read the data from the PYPL table. I created two plots. An interactive plot of the daily returns using hvplot and one for cumulative returns. Next I optomized the data access with advanced SQL queries. Still working with PYPL I accessed the closing prices that were greater than 200 by writing an SQL select statement and read the data from the database into a pandas dataframe then selected the time and close colomms. Then writing a SQL statement to select, order, and limit I found the top 10 daily returns for PYPL. I wrote a SQL query to join each table in the portfolio into a single DataFrame. I also created a dataframe to average all the daily returns for all 4 assets. I used the average daily returns in the DataFrame to calculate the annualized returns for the portfolio and display the annualized return value of the ETF portfolio. 
---

## Technologies

# This project is written with the programming language python. It also uses the libraries Pandas, sqlalchemy, and numpy. The project was written on the Windows operating system.
---

## Installation Guide

```
database_connection_string = 'sqlite:///etf.db'

```
engine = sqlalchemy.create_engine(database_connection_string)
```

```
query = '''
SELECT * FROM PYPL
'''
```
mc_thirty_year = MCSimulation(
    prices_df,
    weights= [.4 , .6],
    num_simulation= 100,
    num_trading_days= 252 * 30
)
```


## Usage

```
etf_cumulative_returns.hvplot(
    title = 'ETF Cumulative Return Values',
    xlabel = 'Year',
    ylabel = 'Returns'
)
---




## Contributors


# Creator of this project is Thomas Burns
# Email is burns235577@gmail.com
---