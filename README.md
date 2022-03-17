# PyBer_Analysis
Incorporating Matplotlib for visual analysis of ride share data. 

## Overview 
Client's ride sharing company(PyBer) had asked to deliver a visual presentation of the ride sharing data from the year 2019. The goal of the project is to assess the relationship between the **variables of rides, fares and drivers** based on the **city types (Urban, Suburban, Rural)**. To that end, Matplotlib Python dependency was incorporated into the analysis to produce multiple graphs that would visually summarize the data across six key metrics: 
- Total Rides 
- Total Drivers
- Total Fares 
- Average Fare per Ride 
- Average Fare per Driver 
- Total Fare by City Type 

### Challenge
A summary DataFrame of the metrics listed above will be used to construct a multiple-line graph that shows the total weekly fares for each city type. This visualization will be used to address any disparities in data among city types. 

The analysis is divided into two code files: 
- [PyBer.ipynb](https://github.com/Fabalin/PyBer_Analysis/blob/main/PyBer.ipynb) - Showcasing statistical analysis and visual quantification of the metrics. 
- [PyBer_Challenge.ipynb](https://github.com/Fabalin/PyBer_Analysis/blob/main/PyBer_Challenge.ipynb) - Summarizing analyzed metrics. 

## Software
Anaconda - 4.11.0
Jupyter Notebook - 6.4.8
Python - 3.7.11

### Highlight of Key Dependencies in Python 
Pandas - 1.4.1
Matplotlib - 3.5.1

## Results
**Bubble Chart of Average Fares vs Total Number of Rides And Drivers by City**
![Bubble Chart of Average Fares vs Total Number of Rides And Drivers by City](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig1.png)
In the chart above, there is a negative correlation between the average fare and the total number of rides and drivers when the data is categorized based on city types. By definition, there is an inherent disparity in population densities of each city type with urban cities having the highest, rural cities having the lowest and suburban cities resting in between urban and rural values (Source: [The Urban and Rural Classifications](https://www2.census.gov/geo/pdfs/reference/GARM/Ch12GARM.pdf)). This inerent disparity becomes appearant in the bubble chart and explains the negative correlation between average fares and total rides as well as average fares and total drivers. Population size itself impacts the supply and demand of the ride share service since higher populations imply higher supply and demand for transportation services such as rideshare apps. This effect is compounded by the geographical spread of the population (population density) as greater spread (lower density) implies longer commute times and consequently, higher fares.  

### Summary Data Frame and Statistical Analysis 
![Summary Data Frame](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/summary_df.png)


There is a description of the differences in ride-sharing data among the different city types. Ride-sharing data include the total rides, total drivers, total fares, average fare per ride and driver, and total fare by city type. 

## Summary 
There is a statement summarizing three business recommendations to the CEO for addressing any disparities among the city types.


