# **The Gold Standard**

![](https://coinweek.com/wp-content/uploads/2011/09/gold_standard.jpg)

## **Background**
The Gold Standard

Currency has played a major role in society for thousands of years. Having an established currency was the mark of humanity's first step towards "functioning modern society". Throughout history, one precious metal has stood as an inherit symbol of monetary value and that metal is none other than gold. 

Around 700 B.C., Lydians made gold into coins, which was the first time in history, or at least the first recorded instance, a society established a standardized currency system for exchange. Gold was always desired and valuable prior to this point, but this act formally solidified its power to function as a monetary unit. 

As more societies emerged around the world, more currencies came into being. Utilizing improved modes of transportation, countries began to engage in commerce with each other, and a global economic framework eventually took shape. 

Countries all established different currencies, yet all mutually recognized gold as a valuable commodity. To facilitate trading, many countries adopted the gold standard or simply settled traded disputes with gold, since all countries had a common conception of gold's value. At the end of the 1800's, a formally written and established internationally gold standard was agreed upon by the majority of developed nations.

Although the gold standard could not survive as a long term monetary system, gold still exists as a physical commodity of value that most developed nations collectively recognize and purchase regularly. 

Gold's significance in the history of commerce and the maintained international understanding makes it the perfect benchmark to compare the buying power of different currencies. Our project aims to draw insights from the buying power of different currencies using gold as the standard to determine each of their value. 

## **Project Procedures**

We first gathered the data for the Average Annual Wages from the majority of developed countries around the world. To begin, We downloaded a CSV file of the necessary data from https://www.oecd-ilibrary.org/social-issues-migration-health/data/oecd-employment-and-labour-market-statistics/average-annual-wages_data-00571-en.

Then we found the data set for the spot price of gold from https://www.investing.com/currencies/xau-usd-historical-data and similarly downloaded the data as a CSV file. Once we found the data sets, we had to import them and define the paths aswell as the variables for each data set
 
After checking the data sets, we dropped unnecessary columns by using the .drop() function

We then proceeded to adjust the numbers from the columns into floats using the str.replace and .astype functions. We plotted the basic line chart for the gold price in USD using the .plot() function. This allows us to visualize the fluctuations of the price of gold over our 20-year time horizon.

To properly present the data, we used the pivot_table function to set the Date as the index and displayed each country in their own individual columns

Next, we used a standard line plot again to illustrate the average salary of each country throughout the 20-year time frame

We divided the annual wage of a given country by the number of weeks in a year times the amount of work hours in a week to determine the buying power of each currency

We downloaded a new CSV file with the hourly wages for each country and added this new data to the existing table

We plotted the new pivot table and used the groupby() and mean() functions to get the average gold price per year 

We created a for loop to divide each country's weekly wage by the gold price average per year and created a new data frame

After creating the new data frame, we used pandas to make a line plot of the annual wages from each country

We calculated the hourly wage by dividing the annual wage by the number of weeks in the year times the hours worked per week

Using a Monte Carlo Simulation, we were able to plot the potential value of gold over the next several years and used confidence intervals to show the bounds

Then we used the pivot_table() function to make an hourly wage data frame

Once we created the new data frame we made a new line plot to visualize the hourly wage of each country




