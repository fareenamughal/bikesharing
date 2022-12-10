# bikesharing

Module 15: NY Citibike with Tableau
___
 
## Overview
___

This bike trip analysis was carried out to assess the viability of the bike-sharing program in Des Moines. An investor wanted to determine whether the investment in Des Moines would be a profitable venture.
 
Data for August 2019 has been used as this is the busiest period for bike sharing. 

To begin with the data which was provided had to be wrangled. The tripduration had to be converted from sting to datetime type. If the questions did not specifically ask the gender data type be changed from integer to string in Tableau, I would have already made the change whilst cleaning up the file. The data cleanup was done using python/pandas code which was run and saved in jupyter notebook  
___

## Results
___

To begin with below are the results of the data cleaning changing the tripduration to datetime data type and eliminating the index column.


![PyBer Fare Summary Jan 1, 2019 to Apr 28, 2019](https://github.com/fareenamughal/PyBer_Analysis/blob/main/Analysis/PyBer_fare_summary_20190101_20190428.png)


Tableau has been used to provide visualizations supporting the analysis. Visualizations are a powerful tool to say a story. The analysis shows that the optimal trip time is approximately 30 minutes, with the largest user group being those of subscribers and males followed by females. Males make up approximately 5/8th of the total whilst females make up a 1/4 and unknown gender approximately 1/8th of the total customers. The largest number of trips during the weekday occur between 5pm to 7pm and 5am to 8am, whilst during the weekend the trips are spread out between 10am to 7pm. The unknown gender customers exceed the male and female.

The pandas/python code written to convert the trip duration from integer to datetime and then generate the revised trip duration csv file can be found as per link here: [nyc_citibike_challenge]([NYC_Citibike_Challenge.ipynb](https://github.com/fareenamughal/bikesharing/blob/main/NYC_Citibike_Challenge.ipynb)]


These results/visualizations, dashboard and story can be found in the tableau link here: [nyc_citibike_challenge Des Moines][(https://public.tableau.com/views/NYCCitibikeTripdataAug-2019/DesMoinesNYCCitibikeTripsAug-2019?:language=en-US&:display_count=n&:origin=viz_share_link)]
___

## Summary
___

The analysis indicates that the servicing of the bikes should bne carried out between midnight and 5am. The other subscribers i.e. female subscribers should be provided with some sort of encouragement or incentive to use bike share more often. It migh be worthwhile to generate ideas to attract female subscribers and users. 
