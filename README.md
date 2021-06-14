# Stock Analysis
## Project Overview
Client asked for a macro to run to determine a stock's volume and return for any given year.  After writing a code that will perform this operation, the next stage was to refactor the code to make it more efficient.  The end goal was to decrease the run time to account for a longer list of stocks under evaluation.

## Results
The first step in the refactoring process was to rewrite the code that calculated the volumes and returns line by line for a given ticker.  The first iteration of the code used two loops, the first loop cycled through the tickers array to perform the calculations for each ticker.  The second loop cycled through the given year's data and performed the calculations.  Refactoring the code paired down the calculations code.  First, the two loops were condensed into one loop through the use of an Index variable.  This variable was set to 0 at the onset and stood as a placeholder for the ticker array numbers (0-11).  After the loop performed the calculations for a given ticker array number, the loop added 1 to the Index so that the next iteration would make calculations for the next ticker array number. Refactored code can be found in the workbook and the improved time stamps are below.

![VBA_Challenge_2017](VBA_Challenge_2017.png)

![VBA_Challenge_2018](VBA_Challenge_2018.png)

## Summary
Refactoring the code can have a few disadvantages such as causing the code to break or even making the code take longer to run.
Advantages include creating code that runs more efficiently or that is simplified so that it is easier to follow.  Refactoring the code also can enable the system to handle more data without crashing.
