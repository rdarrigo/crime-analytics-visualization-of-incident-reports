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

## Plotting the frequency of occurence by the incident hour of day ##

I then plotted the frequency of each of these incidents, grouped by their summarised offence description (Summarized.Offense.Description), by the hour of the day at which the incident occurred (Occurred.Date.or.Date.Range.Start). The points in the visualisation represent actual values, the plot lines for each Summarized Offence Description has been smoothed to emphasise the trend / fit over 24 hours.

Looking at the below visualisation, it was evident that:

* some crimes were more likely to occur in the night hours (6pm - 2am) that during the day (6am - 6pm)
* some crimes were almost equally likely to occur during the day (6am - 6pm) than at night (6am - 6pm)
* some crimes were more likely to occur during the day (6am - 6pm) than in the night hours (6pm - 2am); and
* fairly consistently, the frequency of all crimes reduced in the early hours of the morning (2am-6am)

![Line graph showing top 10 reported crimes and the frequency by the time of day]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/top-10-crimes-by-time-of-day.png)

## 1. Car Prowl, Vehicle Theft incidents occuring mostly at night ##

I then selected the below incidents that looked to have more incidents occur at night. 

* Assault
* Car Prowl
* Vehicle Theft; and
* Property Damage

A similar visualisation was then used to plot the frequency of these incidents across the hour of day. Different plot point shapes were used to provide clarity of the incident type. In addition a black plot line was added to the visualisation, showing the trend of predicted volumes across all three of these summarrised offence description at each hour of the day, along with the respective confidence interval.

It is clear in the below visualisation that Car Prowl and Vehicle Theft incidents are highly likely to occur in the evening. Assault & Property Damage were also more likely to occur in the evening, but this was not as prevalent as Car Prowl and Vehicle Theft. The black trend line also supports this opinion, with more occurances in the evening hours.

![Frequency of Assault, Car Prowl, Vehicle Theft, Property Damage incidents by Hour of Day]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/assault-carprowl-vehicletheft-propertydamage.png)

## Disturbance, Stolen Property & Threats incidents as likely to occur during the day as they are at night ##.

The same visualiation was then used to plot the frequency of incidents of: 

* Disturbance
* Stolen Property
* Threats

This visualisation shows that for these crimes, they are almost equally likley to occur during the day than at night.

![Frequency of Disturbance, Stolen Property & Threats incidents by Hour of Day]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/disturbance-stolenproperty-threats.png)


## Burglary, Fraud & Other Property incidents spikes at around midday and midnight##

Again, the same visualisation was used to plot the frequency of incidents for:

* Burgalry
* Fraud
* Other Property

This visualisation made it clear that these incidents were more likely to occur during the day than at night, but it was also evident that these  

![Frequency of Burglary, Fraud & Other Property incidents by Hour of Day]
(https://raw.githubusercontent.com/rdarrigo/crime-analytics-visualization-of-incident-reports/master/burglary-fraud-otherproperty.png)
