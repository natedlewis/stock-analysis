# stock-analysis

## Overview

The pupose of this project is to further our analysis on some 2017-2018 stocks for Steve by processing data with VBA. We will be expanding the dataset to include the entire stock market over the last few years. Our goal is to refactor our script to loop through the data one time and collect all of the information at increased speeds. We'll then establish whether such tweaks improved execution speeds by comparing our original script to the refactored script.

## Results

**1. Created `tickerIndex` to access the stock ticker index across created arrays.**

> Created three output arrays: `tickerVolumes`, `tickerStartingPrices`, and `tickerEndingPrices`.


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_1.png)

**2. Created a for loop to initialize the `tickerVolumes` to zero, and another that loops over all the rows in the spreadsheet.**

> Before iterating over all the rows, we need to establish any values that must be initialized. Setting the tickerVolumes to 0 ensures that every time we finish analysis on one ticker, the total volume with reset to 0.


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_2.png)

> Increased the current tickerVolumes by using the tickerIndex variable as the index.

> Wrote a nested loop


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_3.png)

**Stock Performance**

> 2017


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_2017_Performance.png?raw=true)

> 2018


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_2018_Performance.png?raw=true)

**Execution times**

> 2017


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2017.png?raw=true)

> 2018


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2018.png?raw=true)

## Summary

The process of refactoring code doesn't involve adding new functionality, but focusues on improving efficinecy. Such goal is met if refactoring enhances the design, makes it easier to understand, helps find bugs, or boosts execution speeds. Budget and time are the primary concerns when performing refactoring tasks. 
 
