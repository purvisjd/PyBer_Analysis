# PyBer Fare Analysis by City Type

##  Overview of Analysis:
This particular analysis is focused on producing a summary of ride-sharing/fare data in areas in which PyBer has drivers and then organizing the data based on city type (i.e., Urban, Suburban, Rural).  Data was read in from both a city data file and a ride data file, merged, and then processed and formatted to provide appropriate analytical data in the form of charts and graphs so that the information may be more readily recognizable and understood.

###  Resources:
*  Data:
    *  [Ride Data](https://github.com/purvisjd/PyBer_Analysis/blob/main/Resources/ride_data.csv)
    *  [City Data](https://github.com/purvisjd/PyBer_Analysis/blob/main/Resources/city_data.csv)
*  Charts created:
    *  [PyBer Fare Summary](https://github.com/purvisjd/PyBer_Analysis/tree/main/Analysis/Pyber_fare_summary.png)
*   Software Used:
    *  Anaconda, Jupyter Notebook 6.3.0

##  Results of Analysis:
In order to assist with not only gathering information regarding current business trends, but also to determine potential future business endeavors and directions, an analysis was completed of ride/fare info for cities in which PyBer currently operates.  The information obtained was extracted from 2 separaate datasets:  ride_data.csv and city_data.csv.  These two files were then merged into a single dataframe and calculations were based on the merged dataset.
![image](https://user-images.githubusercontent.com/85641017/126913983-56edf415-1f3b-490a-9e2d-bad2993a51b9.png)

The focus of this analysis was to gather summary information based on the city type.  The first part of this was done by getting a total number of rides provided by Pyber and grouping them by the type of city.  The same was then done with the total drivers employed by PyBer and the total fares collected was calculated as well, all based on the city type as being either Urban, Suburban, or Rural.  Once these numbers were extracted from the dataset, the average fares per ride and per driver were calculated, keeping the results sorted and grouped by city type.  Once all of the above information was obtained, the following summary data was loaded into a new summary dataframe to give a breakdown of the information:
![image](https://user-images.githubusercontent.com/85641017/126914034-35cbae6b-702a-436d-af98-56c3fdaa06f6.png)

To provide a more visual representation of the acquired data, a multiple line plot was created based on the same information to show the total weekly fares for each type of city.  To accomplish this, a new dataframe was created based on the same information, setting the index on the city type and date information obtained from the raw data.  Once this was complete, the fare data was again summed to provide summary data for the plot graph.  The data was then further narrowed to cover a specific date range of 01/01/2019 to 04/28/2019, displaying the weekly summary info for each week within that date range.  This information was then taken and translated into a line graph to provide a visual representation of the differences between the city types:

![image](https://user-images.githubusercontent.com/85641017/126914090-dac3e822-66f3-4647-8ad5-e8044356c7e7.png)

Some significant differences can be observed right away given the data being worked with.  Urban fares represent a significant portion of PyBer business as evidenced by representing the highest number of total rides, total drivers, and total fares collected.  However, when the totals are averaged out per ridce and per driver, the rural rides represent the highest amounts by approximately $10/ride and approximately $39/driver.  This would indicate that while there are fewer rides being provided in those rural cities, they would appear to be more lucrative.  This could be due to average distance of rides, but further evaluation including that specific data would be needed in order to make such a determination.  When the line graph is viewed, the gross number difference is immediately apparent as is the relative consistency for all types of cities with regards  to rides with one notable exception.  Looking at the included line graph, it appears that there is a significant dip in business for both urban and suburban rides around the first week of April whereas the rural rides do not appear to suffer such a dip in business.  Further analysis regarding circumstances around that specific date range would be required in order to make an accurate analysis as to the cause for this significant drop in numbers.  


##  Summary
A cursory view of the data demonstrates that there is a significant disparity with regards to overall numbers between the three types of cities in which PyBer operates.  There would appear to be significant room for growth and a potential for increased revenue by increasing the number of drivers within the rural areas, potentially increasing the number of rides and, ultimately, the amount of fares collected.  Further research is also recommended to assess how much distance impacts the revenue received from fares and consider the potential for establishing a minimum distance/fare per ride, particularly for the urban drivers to increase their individual collections as well as the overall collections for that area of business.  Based on the overall impression from this summarized information, while urban areas represent the most immediate growth potential, focusing more on the rural areas could also provide significant increases in overall revenue.  
