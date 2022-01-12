# stock-analysis

## Overview

The pupose of this project is to further our analysis on some 2017-2018 stocks for Steve by processing data with VBA. We will be expanding the dataset to include the entire stock market over the last few years. Our goal is to refactor our script to loop through the data one time and collect all of the information at increased speeds. We'll then establish whether such tweaks improved execution speeds by comparing our original script to the refactored script.


## Method

**1. Create a `tickerIndex` variable and set it equal to zero before iterating over all the rows, along with three output arrays.**

* Three output arrays are declared
    * `tickerVolumes`
    * `tickerStartingPrices`
    * `tickerEndingPrices`

* Their purpose is to store values that we can later reference by the `tickerIndex`.
* By default, an array is indexed beginning with zero, so the upper bound of each array is 11 rather than 12.


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_1.png?raw=true)

---

**2. Created a for loop to initialize the `tickerVolumes` to zero, and another that loops over all the rows in the spreadsheet.**

* Before iterating over all the rows, we need to establish any values that must be initialized. 
* Setting the tickerVolumes to 0 ensures that every time we finish analysis on one ticker, the total volume will reset to 0.


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_2.png?raw=true)

---

**3. Within the for loop set above, I wrote a script that increases the current `tickerVolumes` by using the `tickerIndex` variable as the index.**


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/resources/VBA_Challenge_2_Code_3.png?raw=true)

---

**4. I then assigned prices to `tickerStartingPrices` and `tickerEndingPrices` by writing an if-then statement that checks if the current row is the first/last row with the selected `tickerIndex`.**


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/Resources/VBA_Challenge_2_Code_4.png?raw=true)

---

**5. The final script should increase the `tickerIndex` if the next row’s ticker doesn’t match the previous row’s ticker.**


![name-of-you-image](https://github.com/natedlewis/stock-analysis/blob/main/Resources/VBA_Challenge_2_Code_5.png?raw=true)


## Results

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

Clean code is tends to be easier to tweak, easy to read, and required less maintience work. You can avoid facing issues down the road by assessing the refactoring process early on.
 
