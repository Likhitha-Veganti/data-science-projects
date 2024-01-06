# Flight Gain Analysis for United Airlines

## Project Statement

This project explores the gain per flight for United Airlines (UA) using data from the nycflights13 package. The objective is to investigate how much quicker flights end up being than planned, measured by the net gain, which is the difference between departure delay and arrival delay. The analysis employs confidence intervals, hypothesis tests, and exploratory data analysis to address the following questions:

1. Does the average gain differ for flights that departed late versus those that did not? What about for flights that departed more than 30 minutes late?
2. What are the five most common destination airports for United Airlines flights from New York City? Describe the distribution and the average gain for each of these five airports.
3. Calculate the gain per hour by dividing the total gain by the duration in hours of each flight. Does the average gain per hour differ for flights that departed late versus those that did not? What about for flights that departed more than 30 minutes late?
4. Does the average gain per hour differ for longer flights versus shorter flights?

## Executive Summary

In this analysis, we filter the nycflights data to focus on United Airlines flights and introduce new variables, including late, very_late, gain, and gain per hour. The exploratory data analysis involves boxplots, histograms, and statistical tests to answer the project's questions. Here's a summary of key findings:

### 1. Average Gain for Delayed Flights

- Late vs. Not Late: Permutation tests and t-tests suggest a significant difference in net gain between flights that are delayed and those that are not, with non-delayed flights having a higher average gain.

- Very Late vs. Not Very Late: Similar findings indicate that flights not delayed by 30 minutes or more have a higher average gain than very late flights.

### 2. Most Common Destination Airports

- The five most common destination airports for UA flights from NYC are IAH, ORD, SFO, LAX, and DEN.

- Detailed distributions and average gains for each airport are presented, showing normal distributions with various skewness.

### 3. Average Gain per Hour for Delayed Flights

- Late vs. Not Late: Permutation tests and t-tests reveal a significant difference in gain per hour between late and non-late flights, with non-late flights having a higher average gain per hour.

- Very Late vs. Not Very Late: Similar results indicate that flights not delayed by 30 minutes or more have a higher average gain per hour than very late flights.

### 4. Gain per Hour for Longer and Shorter Flights

- Permutation tests and t-tests show a significant difference in gain per hour between shorter and longer flights, with shorter flights having a higher average gain per hour.

## Appendix

Code snippets are provided for each step of the analysis, including data filtering, visualization, and statistical testing. The code is implemented in R using libraries such as ggplot2, tidyverse, nycflights13, and moderndive.
