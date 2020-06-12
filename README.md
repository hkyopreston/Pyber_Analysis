# Pyber Analysis Challenge 
## Module 5

The purpose of this analysis is to create a high level summary DataFrame. This high level summary will include key metrics for Pyber based on city type (Urban, Suburban, and Rural). Along with the Summary Dataframe, this analysis created a visual line graph to show the Total Fares by City Type for a certain period of time. I analyzed the data by first loading, reading, and inspecting the data. Then I created Dataframes for city information and ride information, merged the DataFrames, and then conducted my analysis using calculations on the merged DataFrame.
In the Summary DataFrame, you can easily see that Rural cities have a much higher Average Fares than Suburban and Urban Areas. There is a negative correlation between Number of Rides and Numbers of Drivers to Average Fares. This means that urban cities, with better accessibility to Pyber Drivers will have more rides, but the fare will be cheaper. 

### The image below shows the Summary DataFrame

<img src ="https://github.com/hkyopreston/Pyber_Analysis/blob/master/Summary%20DataFrame.png?raw=true"></img>

The line graph shows that how total fares by city types flow during the months of Jan-April. It seems that in all city types, the ebs and flows are somewhat similar. All three lines peak right before March. The reasoning is unknown, but one could assume that Pyber has more sales in colder weather, when people are not as willing to walk or take public transit. The spikes could also be due to holidays or events that are congruent no matter the city type. 

### The image below shows the line graph. 

<img src ="https://github.com/hkyopreston/Pyber_Analysis/blob/master/Total_Fare_by_City_Type.png?raw=true"></img>


---------------------------

The main difficulties I encoutered was with the line graph. Converting the Date index to a DateTime data type was difficult for me, as there was many differing syntax guidelines in converting data types. I also struggled with created a new pivot DataFrame with the converted index and specific columns. Creating a Pivot Table was a new task so it took some research to create it. I used stack overflow to find examples of both the things I struggled with. 

---------------------------

I would recommend that there be a push to employ more drivers in suburban and possibly rural areas. There would need to be more research done to see if demand exists for Pyber rides first. Increasing the number of drivers in those areas could increase the total number of rides and decrease the cost to the rider. 
In order to gain more insight, the following analyses could be done:

  * Analyze the total fares by city type on a weekly basis for the entirety of 2019. 
      * This would be similar to the previous line graph in that a weekly pivot DataFrame would need to be created for all of  2019. This could give Pyber a better depiction of when drivers are in more demand. 
      
  * Analyze Suburban and Rural cities to see if any of them need an influx of drivers
      *  A DataFrame for both Suburban and Rural city types would need to be created. Possibly a pivot DataFrame that shows the city type and then each city within those types. The total fares per city would need to be calculated using the groupby() and sum() functions. The total drivers for each city grouped by city types will also need to be calculated. 


