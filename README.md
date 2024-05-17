# Team Tornado Alleycats
### Tornado Alley is a region in the United States that sees more tornadoes per year than any other part of the world. 
The unique geography of the United States - from its proximity the jet stream, multiple sources of ocean temperature air, and vast valley in the middle of the country - create the ideal breeding ground for tornadoes and other extreme weather events. Tornado Alley refers to the Great Plains region of the US (Iowa, Nebraska, Kansas, Oklahoma, north Texas, etc) but the greatest clustering of tornadoes has seasonality as well, moving southeast in the colder seasons and northwest as the weather warms.<sup>[1]</sup> 

That said, the general trend of tornadoes may also be moving. The etiology of this behavior is still debated,<sup>[2]</sup> but the impacts are much more immediate. If extreme weather events are generally moving more southeastwardly, then they are also traveling towards more densely populated areas of the country. Not just more densely populated, but towards areas with a higher proportion of mobile homes and buildings not designed for this kind of weather. This may lead to more property damage and possibly to more weather-related fatalities.

We want to understand if this trend is happening and what the impacts will be. We are interested in modeling the potential impact to weather-related fatalities if storms are indeed moving southeast. We also want to understand if the reported increase in tornado "clusters" is moving southeast as well and if that impacts the damage done to those areas. 

## Sources
#### Storms and Tornadoes: 
https://www.ncei.noaa.gov/pub/data/swdi/stormevents/csvfiles/  
We have written a custom script to scrape the data from this NOAA source and compile the last 70 or so years of storm data into one master file. 

#### Census: 
https://www.census.gov/  
We will be using the US Census data to map population densities of affected areas

## KPIs and Stakeholders
This report is most important for residents of the affected areas but could also be used by organizations like FEMA, the American Red Cross, and organizations involved in weather preparedness. We are most interested in the impacts of these storms' migration, so our KPIs are aligned to this:
* Accuracy of our model's "Weather-Related Fatality Field" or WaRFF compared to actual storms. Our model should outperform a baseline of "mean fatalities for a given EF intensity tornado" for a given coordinate area
* Predicting the geographical and calendar shift in tornado intensity 

<sub>[1] https://www.nature.com/articles/s41612-018-0048-2.pdf </sub>  
<sub>[2] https://www.nytimes.com/article/tornado-climate-change.html </sub>