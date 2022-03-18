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
- Anaconda - 4.11.0
- Jupyter Notebook - 6.4.8
- Python - 3.7.11

### Highlight of Key Dependencies in Python 
- Pandas - 1.4.1
- Matplotlib - 3.5.1

## Results
**Bubble Chart of Average Fares vs Total Number of Rides And Drivers by City**
![Bubble Chart of Average Fares vs Total Number of Rides And Drivers by City](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig1.png)
In the chart above, there is a negative trend between the average fare and the total number of rides and drivers when the data is categorized based on city types. By definition, there is an inherent disparity in population densities of each city type with urban cities having the highest, rural cities having the lowest and suburban cities resting in between urban and rural values (Source: [The Urban and Rural Classifications](https://www2.census.gov/geo/pdfs/reference/GARM/Ch12GARM.pdf)). This inerent disparity becomes appearant in the bubble chart and explains the negative trend between average fares and total rides as well as average fares and total drivers. Population size itself impacts the supply and demand of the ride share service since higher populations imply higher supply and demand for transportation services such as rideshare apps. This effect is compounded by the geographical spread of the population (population density) as greater spread (lower density) implies longer commute times and consequently, higher fares.  

### Summary of Key Metrics and Statistical Analysis 
![Summary Data Frame](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/summary_df.png)
Within the data analyzed per city type, there were: 66 urban cities, 36 suburban cities and 18 rural cities. This is approximately a decrease of 2x from each city type ranked (urban, suburban and rural). The average fares per ride and per driver increase as population density decreases because there is less demand for the service. This deters drivers from going to rural cities and thus the supply decreases in turn. This drives up the good of the service as transportation is crucial regardless of the city type. Despite the high average fares in rural areas, drivers are less likely to commit to rides because the long commute time of not only the ride itself, but also the time required for the driver to commute to the driver and also to their next rider. This impedes the ability of the driver to generate a large volume of daily rides in order to gain more profit. 

#### Total Rides per City Type - Percentages and Statistical Summary 
![Total Rides by City Type](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig6.png)
![Ride Count Data](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig2.png)
Overall the spread of the rides between each city type is as expected. The differnces become more pronounced when comparing urban and rural cities. The differences between the urban and suburban cities isn't as drastic compared to the differences between rural and the rest of the city types. This reflects the disparity within the demand of the ride share service between city types. The whiskers and boxes become bigger as population size increases from rural to urban suggesting more variations between each city in urban cities than the rural cities. Without the population data it is difficult to accurately elucidate the culprit beind the disparities observed. 

- Urban cities have the highest ride count 1,625, which represents 68.4% of the gross total rides. The median is 24 rides per city with the outlier West Angela City having 39 rides. the lowest ride count for urban cities is 12. 

- Suburban cities have 625 total rides representing 26.3% of the gross total rides. This is 2.6x lower than urban cities. The median rides per city is around 17 rides and is below the lower quartile of urban city rides. 
 
- Rural cities have the lowest total rides of 125, representing 5.3% of the gross total rides. This is 13x lower than urban cities and 5x lower than suburban cities. The median rides per city is around 6 rides which is well below the lower quartile and the minimum number of rides in suburban cities.    

#### Total Drivers per City Type - Percentages and Statistical Summary 
![Total Drivers by City Type](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig7.png)
![Driver Count Data](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig4.png)
Overall the differences between the driver counts is more drastic than the ride counts. Especially when comparing the urban city types with the rest of the city types. This analysis reflects the disparity in the supply of the ride share service between each city type. Urban cities have a wide range of driver counts but rural and even suburban cities have similar driver counts between each city. Additionally, when comparing the total number of rides and drivers, there is a decreasing trend based on city size for both metrics. Upon closer look, the total number of driver exceeds the total number of rides in urban cities suggesting that there is more supply than demand on average in urban cities as opposed to the rest of the cities.   

- Urban cities have the most drivers at 2,405, which represents 80.9% of the gross total drivers. The median is 36 drivers per city with a minimum of 3 drivers per city and the maximum of 73 drivers per city. This is a huge range compared to the rest of the metrics. When contrasted with the less drastic spread of the demand (ride counts) in urban cities, there seems to be a disconnect. Despite the availability of demand, there seems to be some cities in which the supply (driver count) can't match the demand. This could be an indicator of possible competing ride share services that influence PyBer's ability to supply its services. 
   
- Suburban cities have 490 drivers representing 16.5% of the gross total drivers. This is 5x lower than urban cities. The median drivers per city is around 16 and is below the lower quartile of urban city drivers. The range of driver counts is bigger than that of the ride count which suggests that despite the demand, the supply can vary. The bubble chart shows 3 cities with high ride counts that do not have high driver counts in rural cities. There could be multiple factors impacting the availability of drivers within each of the suburban cities. For example, the percieved relative wealth of the city that compel drivers to stick to wealthier cities, competition from different ride share apps or the accident/crime rate of some cities that affect the safety of the drivers thus deterring them from providing the service. This also occurs in urban cities as well since the bubble chart displays two cities exhibiting the same relationship between high ride count and low driver count. 
    
- Rural cities have the lowest total drivers of 78, representing 2.6% of the gross total drivers. This is 31x lower than urban cities and 6x lower than suburban cities. The median drivers per city is around 4 which is well below the lower quartile of drivers in suburban cities. The spread of the drivers in rural cities is comparable to the spread of the ride count but the ride count still remains bigger than the driver count based on the median and the upper quartiles. When taken into account that the maximum ride count per rural city is 12, it could explain the lower driver count as the business model does not seem sustainable due to the scarcity of demand.    

#### Total and Average Fares by City Type- Percentages and Statistical Summary 
![Total Fares by City Type](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig5.png)
![Ride Fare Data](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/Fig3.png)
The differences between the each city types is not drastic. The spread remains relatively the same. In contrast to the previous metrics based on the box and whisker plot, there is a trend of average ride fares increasing based on the city type starting from urban to rural cities. This is an inverse of the trend observed in total fares as urban cities have a higher total fare than the rural cities. This 

- Urban cities have an average fare per ride of $24.53 and with a similar median value. The maximum average fare is $44.97 per ride and the minimum fare is $4.05 per ride. The urban fares account for 62.7% of the total fares. These percentages mirror that of the ride count of the cities. 
   
- Suburban cities have an average fare per ride of $30.97 and a similar median value. The maximum average fare is $49.96 per ride and the minumum fare is $12.05 per ride. The suburban fares account for 30.5% of the total fares and the percentages mirror that of the ride count of the cities. On average, the suburban rides cost more than the urban rides and this can be explained by population density and geographical distance of suburban cities. The minimum fare is higher than that of the urban cities which indicates longer commute times or distances that cost more than the urban commutes. 
    
- Rural cities have an average fare ride of $34.62 and a similar but higher median value of around $36. This suggests that there is a slight left skew. Additionally, the spread is greater than those of the rural and the suburban cities. given the small sample size of 18 cities, the differences between individual cities become more pronounced. The maximum average fare is $58.55 and the minimum average fare is $10.11. Although the maximum fare is greater than that of the suburban cities, the minimum fare is slightly lower. When looking at the bubble plot, there is a rural city with a low total number of rides, a relatively average driver count that has low average fares. In this case, the interplay of supply and demand whereby the supply can match and even exceed the scarce demand drags the price of the rides down in order to remain viable. The rural fares represent 6.8% of the total fares. 

#### Total Fares per City Type by Weeks from (Jan. 6th, 2019 to Apr. 28th, 2019)
![Gross Total Fares per City Type](https://github.com/Fabalin/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)
The line graph reveals that the fares for each city type from the beginning of the year to April remains relatively stable overall with slight spikes for all city types. Based on this, there is an peak around the week of February 24th, 2019 indiciating an increase in demand across all city types. This could potentially coincide with a federal holiday (Presidents' Day) weekend where people are more likely to drink and celebrate. 

- Urban cities have an increasing trend from the beginning of the year to Feb. 24th followed by 2 alternating spikes on the month of March that levels out after a final increase. Despite the spikes in March, urban cities contribute the most total fare and is the safest business model for drivers as there is plentiful demand to go around. The lower average fare rate and the lower average fare per driver can be compensated by the constant demand and high ride count in urban cities. This translates to higher driver count in urban cities as profit is more likely. This could also translate to lower fares due to higher competition between drivers and even between ride share services. 

- Suburban cities follow a similar trend with a steady increase from the beginning of January with a slight dip on the beginning of February. After the spike in February, there is a relative stable baseline fare rate around March with a slight spike in the middle. Beginning in April, there is a dip on the first week followed by a steady climb through the end of the month. Rural cities have the most steady fare rate out of all of the city types. This is a relatively safe and lucrative business model that is sustainable for drivers, despite the ride count being lower than that of urban cities. 

- Rural cities have the most spikes and is less stable and sustainable than rural cities despite the high average fare per ride and average fare per driver because the demand is not as high due to its low population density. Due to this, the average fares are higher because they reflect the longer commute time in conjunction with the low supply from the lower driver counts. There are 2 major spikes with 3 minor spikes. January experiences a small spike in the middle of the month. February experiences a spike at the beginning and towards the end of the month. March experiences a small spike in the beginning and then April experiences a major spike during the beginning. 

## Summary 
Despite of the inherent differences in population density and size, the demand for ride share services still exist across all city types. Although the demand is lower in the rural areas, the supply itself is considerably smaller than the demand. Driver outreach and incentives must be enacted to ensure that the supply remains consistent for potential rides. Additionally, accurately assessing the demand in areas with low population density through research is important to understand individual motivations towards using the ride share apps. More research needs to be done in target cities with particularly low driver counts but high ride counts to assess the quality of user experience, improvements should be made to catering to riders and drivers to decrease possible competition from other ride share apps. Conversely, discouraging services in rural areas while encouraging serivce in suburban areas would also be viable as the rural fares only represent 6.8% of the total fares but suburban fares represent 30.5% of the total fares. This would focus all efforts to urban and suburban cities where the demand and the supply is well established. 

- Promote incentives using bonuses in conjunction with optional quotas for drivers to exclusively take riders to and from suburban and rural areas. It is important to ensure that the quotas are optional since mandatory quotas can ultimately impede the driver's freedom to source their customers and drive them towards other ride share apps. For example: one ride to targeted rural cities on a monthly or bi-monthly basis can provide bonus pay. This method can also be used to promote intercity commutes between urban and the rest of the city types to ensure that drivers can meet personal daily ride quotas while conducting outreach in cities with less ride volumes. 

- Increase company investment in suburban and rural campagins to promote the ride share app in cities with existing ride data. This would increase the app's visibililty in areas with known market viability to promote further use of the app. 

- Provide drivers with the materials to promote the ride share app. For example, a light up sign reminiscent of a taxi with PyBer's logo is an easy way to promote and advertise the company since the drivers are able to promote the ride share along their route. 
