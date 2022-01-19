# NY Parking Tickets Exploratory Analysis

 Language Used : Python ,PySpark

 Tools Used : Spark 

## Problem Statement

 In an attempt to scientifically analyse this phenomenon, the NYC Police Department has collected data for parking tickets. Of these, the data files for multiple years are publicly available on Kaggle. We will try and perform some exploratory analysis on a part of this data. Spark will allow us to analyse the full files at high speeds as opposed to taking a series of random samples that will approximate the population. For the scope of this analysis, we will analyse the parking tickets over the year 2017
 
## Tasks Performed
 
### Examine the Data
 
 1. Find the total number of tickets for the year.
 2. Find out the number of unique states from where the cars that got parking tickets came. (Hint: Use the column 'Registration State'.)
 3. There is a numeric entry '99' in the column, which should be corrected. Replace it with the state having the maximum entries. Provide the number of unique  states again.
 4. Display the top 20 states with the most number of tickets along with their ticket count.

### Aggregation tasks

 1. How often does each violation code occur? Display the frequency of the top five violation codes.
 2. How often does each 'vehicle body type' get a parking ticket? How about the 'vehicle make'? Find the top 5 for both.
 3. Let’s try and find some seasonality in this data:
      1. First, divide the year into 4 seasons, and find the frequencies of tickets for each season.
      2. Then, find the three most common violations for each of these seasons. 
 5. The fines collected from all the instances of parking violation constitute a source of revenue for the NYC Police Department. Let’s take an example of estimating this for the three most commonly occurring codes:
      1. Find the total occurrences of the three most common violation codes.
      2. Then, visit the website:http://www1.nyc.gov/site/finance/vehicles/services-violation-codes.page. It lists the fines associated with different violation codes. They’re divided into two categories: one for the highest-density locations in the city and the other for the rest of the city. For the sake of simplicity, take the average of the two. 
      3. Using this information, find the total amount collected for each of the three violation codes with the maximum tickets. State the code that has the highest total collection (only based on the top 3 tickets).
      4. Find the top 3 states that have the highest ticket revenue based on the top 3 violation codes alone. 
      5. What can you intuitively infer from these findings?
 
