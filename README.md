# bikesharing

Module 15: NY Citibike with Tableau
___
 
## Overview
___

This bike trip analysis was carried out to assess the viability of the bike-sharing program in Des Moines. An investor wanted to determine whether the investment in Des Moines would be a profitable venture.
 
Data for August 2019 has been used as this is the busiest period for bike sharing. 

To begin with the data which was provided had to be wrangled. The tripduration had to be converted from sting to datetime type. If the questions did not specifically ask the gender data type be changed from integer to string in Tableau, I would have already made the change whilst cleaning up the file. The data cleanup was done using python/pandas code which was run and saved in jupyter notebook.

Thereafter, the data was uploaded into Tableau Public to generate the visualizations. A number of visualizations have been generated of which can be viewed in the Images folder. Three dashboards have been generated using the visualizations, each states a story and make up my Tableau story which can be viewed as per link to my tableau story as belwo.

[NYC Citibike Tripdata Aug-2019](https://public.tableau.com/views/NYCCitibikeTripdataAug-2019/DesMoinesNYCCitibikeTripsAug-2019?:language=en-US&:display_count=n&:origin=viz_share_link)
___

## Results
___

Results can be divided into two sections:
A. Data cleaning/wrangling required before any analysis can be done.
B. Analysing and generating the visualizations to support the story or to arrive at rational conculsion.

___

### A. Data cleaning
___

The pandas/python code written to convert the trip duration from integer to datetime and then generate the revised trip duration csv file can be found as per link here: [NYC Citibike Challenge python code]([NYC_Citibike_Challenge.ipynb](https://github.com/fareenamughal/bikesharing/blob/main/NYC_Citibike_Challenge.ipynb)]

Below are the results of the data cleaning changing the tripduration to datetime data type and eliminating the index column.

![Revised NYC Citibike csv](https://github.com/fareenamughal/bikesharing/blob/5082e0ac1987257a5e8bb1d4bd9399a949494e53/Images/screenshot_nyc_citibike_rev_csv_file.png)
___

### B. Analysing and generating the visualization using tableau to support the story
___

Tableau has been used to provide visualizations supporting the analysis. Visualizations are a powerful tool to say a story. I have analysed the data abd providded my findings via three tableau dashboards, each focuses on a specific area.

 #### 1. Dashboard for trip durating

![Trip Duration Dashboard](https://github.com/fareenamughal/bikesharing/blob/d2c48f22611901c59f3145b5229a858b611e676a/Images/Dashboard_1_Trip_duration.png)
The analysis shows that the optimal trip time is approximately 30 to 40 minutes. The largest number of trips during the weekday occur between 4pm/5pm to 7pm  and 6am to 9am. During the weekend the trips are spread out between 10am to 7pm. 
Males are the largest users followed by females and unknowns respectively.


#### 2. Dashboard analysing the usage time


![Usage Time or Heatmap Dashboard](https://github.com/fareenamughal/bikesharing/blob/10b5c10cb719578adf8dcd124ddd7c60cb278cc4/Images/Dashboard_2_Usage_time.png)

This visualtization supports the heavy usage time of 4pm/5pm to 7pm  and 6am to 9am as seen in the trip duration visualization. However, here we take a deeper dive into the breakdown between males, females & unknowns as well as we analyse the usage based on the day of the week. It is clear that males are the larges user group, their usage is heavier on Thursdays and Fridays and Mondays and Tuesday. 

For females, heaviest usage periods are around 8am and 5pm to 6pm during weekdays, 12pm to 5pm on Sundays & 10am to 6pm on Saturdays. Females use bikes more on Thursdays, followed by Tuesdays and Mondays.

The unknowns use bikes more during the weekends with Saturday 10am to 7pm being the busiest, followed by Sundays at 11am to 5pm. During the week days 5pm to 6pm is when unknowns use bikes with Thursdays and Fridays being slightly busier followed by Mondays and Tuesdays.

During the weekend,bike usage by the unknown geneder exceeds bike usage by males and females. 

In another visualizations not included here, it can be seen that males make up approximately 5/8th of the total, whilst females make up a 1/4 and unknown gender approximately 1/8th of the total customers. The largest user type being those of subscribers at approx.80% and customers being approx. 20% of tottal user types. 


#### 3. Dashboard analysing the top starting and ending locations


![Location Dashboard](https://github.com/fareenamughal/bikesharing/blob/10b5c10cb719578adf8dcd124ddd7c60cb278cc4/Images/Dashboard_3_Start_End_Locations.png)

The stating and ending trip locations visualization provide important start point and end point information. It also indicates the exact location on the map for the various stations. As can been seen from the visualizations, the heaviest usage for starting and ending points for trips is the same for the top 6 stations/locations. This is important so as to ensure that bikes are adequately supplied for starting locations and distributed to other stations for ending locations stations. The map can provide an idea of which locations have a shortage or an oversupply and the logistics can be planned out appropriately.
___

## Summary
___

The analysis indicates that the servicing of the bikes should bne carried out between midnight and 5am. The other subscribers i.e. female subscribers should be provided with some sort of encouragement or incentive to use bike share more often. It migh be worthwhile to generate ideas to attract female subscribers and users. The unknown user category can also be provided with incentives to increase bike usage all through the week. There is perhaps need to investigate further the reason for the different usage patterns by the 3 gender types. This information would be important to tailor out incentives to attract each gender type.

In the 3rd dashboard visualizations about start and end locations, in the results section above, it is evident the top 6 starting locations are also the top 6 ending locations. This makes it relatively easy to schedule the bike maintenance in these locations as there will be no need to transfer bikes in and out of these locations to fulfill the demand and supply issues. However, further analysis needs to be done identifying the specific timiming at these stations. More importanly, the other stations, not in the top 6, need to be reviewed both for timing, volume, demand and supply and this needs to be mapped out into a heatmap and scattemap to come up with a plan to sort out any supply & demand logistic issues as and when these arise.


