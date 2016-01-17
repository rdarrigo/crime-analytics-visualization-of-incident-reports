# Vehicle Theft & Car Prowl most likely to occur at night during summer months in Seattle

Using the Seattle Summer 2014 dataset, I wanted to investigate the times that crimes were committed to hopefully uncover patterns, such as particular crimes being more likely to be committed in the day or at night.

Firstly, I decided to focus on the 10 most reported crimes in the data. I subsetted the data so that it only contained the following types of reported incidents.

| Summarized.Offense.Description | Numer of reported incidents |
--------------------|------|
| CAR PROWL         | 6230 |
| OTHER PROPERTY    | 3755 |
| BURGLARY          | 3212 |
| VECHICLE THEFT    | 3057 |
| PROPERTY DAMAGE   | 2365 |
| ASSAULT           | 2018 |
| FRAUD             | 1473 |
| DISTRURBANCE      | 1333 |
| THREATS           | 1178 |
| STOLEN PROPERTY   | 1136 |
[Top 10 reported crimes by volume in Seattle Summer 2014 dataset]

I then plotted the frequency of each of these incidents by their summarised offence description (Summarized.Offense.Description), by the hour of the day at which the incident occurred (Occurred.Date.or.Date.Range.Start). The points in the visualisation represent actual values, the plot line for each Summarized Offence Description has been smoothed to emphasise the trend / fit over 24 hours.

![Line graph showing top 10 reported crimes and the frequency by the time of day]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/top-10-crimes-by-time-of-day.png)

Looking at this visualisation, it was evident that some crimes were more likely to occur in the evening (6pm - 2am), some were more likely during the day than at night (6am-6pm) and all crimes were less likely to occur in the early hours of the morning (2am-6am)

## Car Prowl, Vehicle Theft ncidents occuring mostly at night ##

The same visualisation was then used to only plot the frequency of Car Prowl, Vehicle Theft and Property Damage. In addition a black plot line was added to the visualisation, showing the trend of predicted volumes across all three of these summarrised offence description at each hour of the day, along with the respective confidence interval. The black trend line along with each data point show that these crimes are most likely to occur in the evening.

This was most prevalent in Car Prowl and Vehicle Theft.

![Line graph showing crimes most likely to occur in the evening]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/crimes-prevalent-in-the-evening.png)

## 

The same visualiation was then used to plot the frequenct of Other Property, Burglary, Assault, Fraud, Disturbance, Threats and Stolen Property. Plotting the remaining crimes showed the trend of these crimes more likely to either: 

- occur more likley during the day, than the evening.
- occur consistently throughout the day and evening.


![Line graph showing crimes most likely to occur in the evening]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/disturbance-stolenproperty-threats.png)
