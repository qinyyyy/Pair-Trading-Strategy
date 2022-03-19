# PairTrading
This project examines the impact of a pair trading algorithm using the absolute difference of the ratio of two stocks price in consecutive days.

We pull the stock data from the EOD Historical Data website, populate five SQL tables and store them in the Sqlite3 database. After that, we do the backtest and calculate Profit and Loss. Finally, we allow the user to input prices of two stocks to manually test the performance of pair trading.

We Use C++ to build the code framework, download data and invoke SQL to populate the database, and we mainly use SQL to implement the Backtesting and Calculate Profit and Loss. 
![image](https://user-images.githubusercontent.com/88140638/159142054-ec30ca31-b52c-4226-bf19-f18fb9a6436d.png)

Conclusion:

The profit and loss do not show significant evidence that this pair trading strategy can earn profits.
This strategy considers the absolute value of difference of pairs ratio, and thus ignore which day the ratio is larger. A more reasonable strategy is to consider the mean reverting process of the spread.
In this way, the algorithm does not provide a logic way to make profits. Further steps include taking the positive and negative difference into consideration.
