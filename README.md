# UFO-Sightings-Data-Visualization
The skies above us hold more than just Sun, Moon, Stars and Satellites. The phenomenon of unidentified flying objects (UFOs) continues to intrigue and mystify. Reports of unexplained aerial sightings have been a part of human history for centuries, and they remain an area of public interest and scientific investigation. With countless sightings reported each year, the USA stands out as a hotspot for such unexplained events followed by Canada. I’ve used a couple of data sets from NUFORC database and one data set from OpenFlights. we turn a jumble of latitudes and longitude into a clear path. By utilizing data visualization techniques, we work some magic with data transformation, sorting and organizing information so it makes sense. Plus, we use R Scripts that's great for stats and graphs, to help us see the big picture by analysis to find patterns and occurrences of UFO sightings across the United States. By marrying the OpenFlights data with reported UFO sightings, we're charting a course to possibly explain the unexplained.
# Research Questions:
1. What are the spatial patterns of UFO sightings across United States, Canada and are there any notable concentrations or dispersions of sightings in relation to geographical features or population centers?
2. What are the trends in UFO sighting reports in the United States, Canada and how do the frequencies of these reports vary on a yearly, monthly, and daily basis?
3. What are the distribution patterns of UFO sightings in terms of the reported shapes, and is there a predominance of specific shapes in the reported sightings across different regions of the United States?
4. How does the reported duration of UFO sightings vary across different incidents, and are there identifiable patterns in the lengths of these events that could provide insights into UFO activity?
5. How have patterns of UFO sightings evolved geographically and temporally over recent years, and is there evidence of concentrated activity in specific regions that correlates with changes over time?
6. What are the global patterns in the distribution of airports, and how do geographic factors influence the spread of airports around the world?
7. What is the frequency of UFO sighting reports within various distance ranges from the nearest airport, and do sightings tend to occur more often closer to or farther from these airport locations?
 8. Future Research Questions:
•	Are there discernible patterns in UFO sighting reports that align with commercial airplane travel routes, based on the starting and ending coordinates of flights, and what does this imply about the nature of these sightings?
•	How do weather conditions influence the frequency and geographical distribution of UFO sightings?

Methodology:
Data Sources:
For this analysis, I have collected data from various sources like NUFORC site, Data.World Site and OpenFlights. The dataset includes information on Date/Time the incident was reported, Country, City, State, Shape, Latitude, Longitude, Duration of Event, etc.
 
. ![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/5e2454a8-8362-4065-8aa5-8193c4be4035)

Data gathered from the following sources:
1.	National UFO Reporting Center Reports: This dataset contains information regarding Parse out date and time, and year, month, day, hour, minute, City, State, Shape and Duration.
2.	UFO Sights 2016 US and Canada:  This dataset contains the summary of the curated data extracted from the NUFORC database containing UFO sights from US and Canada during 2016. The information included Date/Time the incident was reported, Country, City, State, Shape of the UFO, Latitude, Longitude.
3.	Airport database: The OpenFlights Airports Database contains over 10,000 airports, train stations and ferry terminals spanning the globe. This dataset contains information regarding Name, Country, City, Time zone, Latitude, Longitude and Altitude.
4.	Calculated Data:  This Dataset is the extended version of UFOs_coord with added column of nearest airport distance calculated and updated using R script

Data Source References:
1. https://data.world/khturner/national-ufo-reporting-center-reports
2. https://data.world/aarranzlopez/ufo-sights-2016-us-and-canada
3. https://openflights.org/data.php





Data Preprocessing:
Before creating visualizations, the data underwent preprocessing to clean and transform it. This included handling missing values, removing unused columns, adding new columns, and aggregating data by using R scripts.


Analysis:
1.	What are the spatial patterns of UFO sightings across United States, Canada and are there any notable concentrations or dispersions of sightings in relation to geographical features or population centers?
   
 ![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/001c619e-b7c9-450b-b956-421eaa4176a2)

In this Visualization, we did analysis of UFO sighting reports by mapping the latitude and longitude coordinates on map of UFO sightings.


2.	What are the trends in UFO sighting reports in the United States, Canada and how do the frequencies of these reports vary on a yearly, monthly, and daily basis?
   
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/68c908cd-03ef-4ae8-85da-aa2794cbf186)

Yearly Trends: The line chart shows the number of UFO sighting reports in the U.S. from the early 2000s through approximately 2015. There is a general upward trend in reports from 2000 until around 2012, where it peaks. After 2012, there is a notable decline in the number of reports. The peak in 2012 might have been influenced by popular culture or increased public interest in UFOs around that time. The subsequent decline could be due to various factors including changes in public interest or the availability of new platforms for reporting.
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/7666284c-1c91-4af0-8806-cc6f79263a6b)

 
Monthly Distribution: The second visualization breaks down UFO sightings by month. The line chart indicates that sightings increase significantly in January and then generally decrease through the subsequent months, with minor peaks mid-year. The pie chart reveals that January has the highest percentage of reports, suggesting a possible seasonal pattern where sights are more frequent in winter months.

![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/87c1f41c-1b34-4a72-83ad-a85f40cd63ad)


Daily Distribution: The daily distribution of UFO sightings shows considerable variability. There are specific spikes on certain days of the month, particularly noticeable around the 1st, 15th, and towards the end of the month. This could indicate reporting biases or patterns in when events are observed or recorded. The pie chart for daily distribution does not show a consistent trend, suggesting that daily sightings are relatively spread out throughout the month with no single day overwhelmingly dominating.

There is a clear peak and decline in the frequency of reports over the years examined. The reasons behind these trends could be multifactorial, including media influence, societal interest, and the availability of digital platforms for reporting. There appears to be a seasonal trend with more sightings reported in the colder months, peaking in January. This could be related to longer nights in winter, providing more opportunities to observe unusual phenomena. The spikes on specific days might suggest reporting or observational biases rather than an actual increase in sightings. This comprehensive analysis shows not only the temporal trends in UFO sighting reports but also hints at underlying factors that could influence these observations.

3.	What are the distribution patterns of UFO sightings in terms of the reported shapes, and is there a predominance of specific shapes in the reported sightings across different regions of the United States?

![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/071e397e-0a87-46e8-8abd-35da2cef7466)
 
The stacked area chart we used shows the number of UFO sightings reports by shape each year, spanning several decades. There is a noticeable increase in reports starting from the late 20th century, peaking in the 2000s. The variety of shapes reported has also diversified over the years. Notable among them are shapes labeled as "Light," "Circle," and "Triangle," which show significant increases over time, suggesting that these shapes are more commonly reported than others. The overall upward trend in sightings might be influenced by increasing public interest, more accessible reporting channels, or growing awareness of aerial phenomena.


4.	How does the reported duration of UFO sightings vary across different incidents, and are there identifiable patterns in the lengths of these events that could provide insights into UFO activity?
 ![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/bf910f29-c8e5-4794-8f70-76b947a56a75)

For these visualizations, I used a geographical map and a bar chart for UFO sighting durations, I noticed intriguing patterns in the distribution and duration of UFO sightings across North America. The map shows that sightings are more frequent in densely populated areas like the West Coast, Northeast, and Great Lakes region, which suggests that urban environments with larger populations may see more reports due to the greater number of potential witnesses. The bar chart reveals that most UFO sightings are brief, typically lasting less than 5 minutes, with the most common durations being 1 and 2 minutes. This prevalence of short encounters might indicate that the phenomena observed are generally transient, possibly characterized by quick appearances or movements. Longer sightings over 30 minutes are rare, which could imply that extended observations of UFOs are uncommon, perhaps due to the fleeting nature of the events or biases in reporting shorter, more memorable incidents. My analysis highlights the importance of considering both the geographical and temporal aspects of UFO sightings to better understand the underlying factors influencing these reports.


5.	 How have patterns of UFO sightings evolved geographically and temporally over recent years, and is there evidence of concentrated activity in specific regions that correlates with changes over time?

 ![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/c29fd006-0ea5-467d-b25b-95749ff705fe)
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/46b982fd-bdc7-48db-b246-e831876eca5d) 

 

With the animated charts, I've noticed that UFO sightings concentration varies time to time, where the dense population likely boosts sightings and reports. Temporally, sightings fluctuate, with peaks possibly linked to media coverage or public interest spikes, such as in 2010 and 2017. This suggests that both location and time significantly impact UFO sighting patterns, with activity focused in urban areas and influenced by cultural events.

6.	What are the global patterns in the distribution of airports, and how do geographic factors influence the spread of airports around the world?

 ![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/043368fe-0ead-4ade-8860-36d04a595cdf)
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/e516d52a-f37f-4f20-81f9-e20342ed3635)
 
With the use of  Maps, we located the Airport coordinates all over the world and for USA and Canada to link the data with UFO sighting to find meaningful insights and patterns.

7.	What is the frequency of UFO sighting reports within various distance ranges from the nearest airport, and do sightings tend to occur more often closer to or farther from these airport locations?
 
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/f6881e79-ca57-4ff6-88d7-4bcb822024d4)
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/192e7446-4ec3-4956-88bc-7f1da0c79232)
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/f8dc5ad5-9374-4f9a-a6c4-c8590731e31b)
![image](https://github.com/manikanta-yaswanth/UFO-Sightings-Data-Visualization/assets/161633030/743a2402-1875-4246-94da-db80fb9a0946)
 
 
 

From these charts, I've observed that UFO sightings are reported at varying distances from airports, with a noticeable concentration of cases both very close to and at moderate distances from airports. The first chart shows a high frequency of reports close to airports, which then tapers off as the distance increases, suggesting that proximity to airports could be a factor in many sightings. This pattern could be due to the higher likelihood of observing unusual aerial phenomena near airports, where air traffic is densest.

Additionally, the charts illustrating the radius of UFO reports near airport locations confirm that sightings are indeed common in areas surrounding airports but also extend outward, covering a wide geographical range. This distribution could be influenced by the high visibility conditions and public alertness in areas near airports.

In summary, while UFO sightings are frequent near airports, they are not confined to these areas and can occur over a broad range of distances, reflecting the widespread nature of these reports. This suggests that while proximity to airports, with their associated air traffic and activity, might increase the chances of sighting unusual phenomena, other factors also play a significant role in the distribution of these sightings.


Conclusion: 
A thorough exploration of UFO sightings in relation to airport proximity has been conducted in this study with a focus on different distances. The findings reveal that sightings are frequent near airports but can occur at a range of distances, and noticeably cluster close to or moderately far from airports rather than being restricted solely to these locations. Such information enhances our understanding of where UFO sightings tend to happen relative to air traffic hubs, highlighting the importance of geographic and operational factors governing their occurrence and distribution. Moreover, it demonstrates how data visualization can be useful for identifying patterns that may support further research on unidentified aerial phenomena (UAPs), thereby helping UFO enthusiasts, researchers, and the public to unravel what seems like complex dynamics behind these events.

