# Querying-a-Database-with-Python
All parts involve using Python to query a SQLite database, dj.db. Use the database provided with the assignment.
Part A – Query tickers with fetchall()
Write Python statements to query the tickers table in the dj.db database. Use the SQL statement:
SELECT id, ticker, name FROM tickers
Place the results in a pandas DataFrame, using the ticker field as the DataFrame row index. Display the
DataFrame.
Part B – Determine the date span of the data
Write Python statements to query the daily_measures table in the dj.db database, and determine the
earliest and latest date of the data in this table. Use the SQL statement:
SELECT min(date) as first, max(date) as last FROM daily_measures
Part C – Query price history with for and Cursor
Write Python statements to query the daily_measures table in the dj.db database, and based on the
returned data, determine the date and closing price of the highest price for Apple stock during the data
available in the database. Use the SQL statement:
SELECT date, closing FROM daily_measures WHERE ticker_id=3 ORDER BY date
Part D – Query price history to determine largest 1-day price percentage moves
Write Python statements to determine the date and price when Apple had the highest one-day percent
change. Use the same SQL statement as in part C, and additional Python (and possibly pandas)
statements to find the result.
