# Causes for Flight Delays in the US from 2010-2020
### by Jordan Mazza

## Introduction
I chose to analyze the Airline Statistics and Delay Causes dataframe provided by Udacity. I downloaded flight delay statistics from January 2003 to September 2020. This dataset started with 288,150 rows and 22 columns.

In terms of data wrangling, I did not need to do too many steps. When I first downloaded the data, some column names had whitespace, so I performed the strip to remove them. Over the course of my analyses, I narrowed the timeframe of my analysis to January 2010 to September 2020. I also dropped some columns I felt were unnecessary or repetitive to my analyses. For example, there were columns for airport code and airport name, so I dropped the airport name column and kept the airport code column.

## Summary of Findings
### Univariate Findings
For univariate exploration, I performed several analyses:
- Two bar charts, one showing number or weather delays per month, the other showing length of weather delays per month.
- Two line charts, one showing total flight delays per year, the other showing percentage of flights delayed per year.
- One bar chart showing the percentage of flights delayed per airline.
- Two waffle charts, one showing percentage of flights in the dataset that were on time, cancelled, and delayed and another showing percentage of delayed flights caused by each variable .
- A series of five histograms showing the distribution of the delay length for each type of delay.

The first bar plot in the analysis shows the number of weather delays per month. I suspected winter months would have more weather, but this plot doesn’t support that. Summer months have higher amounts of weather delays. I also wanted to see if length of weather delay was related to time of year, so I made a similar plot showing length of delay per month; however, the plot still did not follow my prediction. Delays are typically long in winter months, but they are longest during summer months. Since I have a plot that goes into further depth on this analysis under multivariate exploration, I did not include these plots in my presentation in order to keep it concise.

The second set of plots show total flight delays over time, both in total amount, as well as proportionately. Unsurprisingly, the year 2020 has a significant drop in flight delays in both overall numbers, and proportionately. Because travel has ceased for many Americans this year, they are less flights in general; therefore, there are less flight delays. I did include this in my presentation because I felt it relevant to current times.

I then made another bar plot that shows the percentage of flights delayed per airline. While this information is interesting, there could be other variables effecting this graph, such as number of locations (as well as where those locations are) that can play into this result. I had intentions on continuing to analyze this; however, with so many airlines in the dataset (26) and other features of interest, I decided to not continue with these analyses. For the same reasons, I did not include it in the presentation. 

Next, I made two waffle plots, the first showing how many flights were delayed compared to on-time and cancelled flights. Similarly, the second waffle plot shows the breakdown of delay causes out of all delayed flights. The most common delay cause is late aircrafts, while the smallest by far is security delays (it doesn’t even show on the plot). I chose to include this second waffle plot because I find this plot more interesting and relevant to the rest of the presentation.

My last univariate plot is a series of histograms showing the duration distribution in minutes of the five flight delay causes. I used a logarithmic scale for these histograms because they were all incredibly right skewed and had long, narrow tails. The delay types with the longest length on average are carrier, and NAS delays. I did not indlude this in my presentation becuase it would not fit on the slides. 

### Bivariate Findings
For bivariate exploration, I performed two analyses: A heatmap and a Pair Grid of the 5 delay variables to see if there were any relationships among them. I didn’t move forward with any more bivariate analyses because no further insights were apparent when using a different scale or transformation for these plots. All the graphs were readable before transformation, so it seemed redundant to create multiple bivariate plots that portrayed the same information as the Pair Grid plot.

From these graphs, we can see some strong relationships between some of the variables, namely between:
- Carrier and late aircraft (0.905)
- NAS and carrier (0.813)
- Late aircraft and NAS (0.806)
- Weather and late aircraft (0.733)

The weakest correlations were the relationships between security delays and all other delay causes. I would imagine this is because security delays are rare and happen significantly less than all other delays. 

While I find the PairGrid plot easier to understand upon first glance for the average person, I included the heatmap in the presentation because it is more compact and fits better on the slides.
