# Stock_Analysis

# Purpose
The purpose is to perform analysis on different stocks and their performances in year 2017 and 2018. A macro was created in VBA to output calculations for our analysis. An interface was created to allow users to perform these basic functions with the click of a button.

# Results
Below, we see the two stock analysis for both years. The "Total Daily Volume" (which refers to the number of trades of a particular stock) is summed over the course of the year. In the "Return" column, the stocks' price at the end of the year is divided by the price at the beginning of the year and converted to show percentage gain or loss. This indicates the return on investment for a specific stock for the investor with green indicating gains and red indicating losses.

![alt text](https://github.com/anamahmed15/Stock_Analysis/blob/main/Stocks_2017.PNG)


![alt text](https://github.com/anamahmed15/Stock_Analysis/blob/main/Stocks_2018.PNG)

Through conditional formatting, we can clearly see the differences in stock performance for both years. In 2017, only one stock shows a negative return; while 2018 indicated to be a year of lossess for most stocks.

The stock DQ for example shows a drastic swing in performance, indicating it to be a very high risk stock with great fluctuations.

Code refactoring was a major part of this project - the initial analysis was written using a nested for loop. While nested loops are effective, they do come with a price - speed.

![alt text](https://github.com/anamahmed15/Stock_Analysis/blob/main/VBA_Challenge_2017.PNG)


![alt text](https://github.com/anamahmed15/Stock_Analysis/blob/main/VBA_Challenge_2018.PNG)


In the loop below, the computer runs through each record of the data set once for each possible ticker category. In this case, there are only 12 categories and 3013 rows of data. However, in a worst case scenario, each record could be unique, meaning that the computer would run through the x values x amount of times.

![alt text](https://github.com/anamahmed15/Stock_Analysis/blob/main/Nested%20for%20loop.PNG)

To reduce the time, we refractored the code into an array. In this way the computer now needs to access each data row only once. By using pre-sorted data, we are essentially designating a zone, and once the computer recognizes that it has left the "AY" zone, it doesn't have to go check back through those rows to confirm that there are no other values in that range. 
