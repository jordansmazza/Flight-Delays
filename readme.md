# Causes for Flight Delays in the US from 2010-2020
### by Jordan Mazza

## Introduction
I chose to analyze the Airline Statistics and Delay Causes dataframe provided by Udacity. I downloaded flight delay statistics from January 2003 to September 2020. This dataset started with 288,150 rows and 22 columns.

In terms of data wrangling, I did not need to do too many steps. When I first downloaded the data, some column names had whitespace, so I performed the strip to remove them. Over the course of my analyses, I narrowed the timeframe of my analysis to January 2010 to September 2020. I also dropped some columns I felt were unnecessary or repetitive to my analyses. For example, there were columns for airport code and airport name, so I dropped the airport name column and kept the airport code column.