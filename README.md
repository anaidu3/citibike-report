# Unit 18 Homework: Citi Bike Analytics

Data Source: Citi Bike System Data
https://www.citibikenyc.com/system-data

* Raw data and the compiled csv are not included in git hub due to file size restrictions

Methodology (ETL):
* Extracted data from February 2021 - June 2022
* Combined multiple excel files in Jupyter Notebook
* Created a trip duration column
* Cleaned data
* Exported data into a csv file
* Loaded data into a Tableau Workbook for visualization

The following analysis provides a way to visualize and understand the quantity of citi bike rides, when bike rides occur, the duration of rides, and the most popular stations.
The analysis specifically compares data in 2021 to current data in 2022 to gather insight into future citi bike ride patterns.

Report located here: https://public.tableau.com/shared/YT6NK74WB?:display_count=n&:origin=viz_share_link

Research Questions:
* How are the Citi Bike rides doing in 2022 vs 2021? (Quantity of Bike Rides)
* What months or days do riders take rides? (When Bike Rides Occur)
* How long are Citi Bike riders using the bikes for in a single ride? (Duration of Trip)
* Which stations are more popular to start a trip from and end a trip from? (Popular stations)

Time Frame Chosen:
Febrary 2021 - June 2022 was chosen to consider at least a year worth of data to analyze. 
Note, Jan 2021 data was initially extracted, but many columns were either missing or changed between January to February time period.
With initial data exploration, it was assessed that sufficient analysis could be completed without January 2021 citi bike data, and so it was left out for the analysis.
In much of the analysis, January 2022 data was filtered out to compare month by month data accurately.

Analysis:

* Citi Bike Rides
  * The number of rides has increased consistently month to month in 2022 vs 2021
  * Interestingly, there seems to be a seasonal trend in rides taken, which is likely due to riders more willing to ride a bicycle when it is not too cold outside. 
  * This seasonal trend will likely continue in 2022, such that the number of rides will be larger than in 2022, but the number of rides will still decrease in the winter months.
  * There is not a clear trend on more popular day to take a citi bike, but the general trends from 2021 follow the same trends seen in 2022 for each month.
    * Total Number of Trips from Feb 2021 - Dec 2021: 629,319
    * Total Number of Trips from Feb 2022 - June 2022: 329,063

* Citi Trip Duration
  * Even though there have been more rides and more accumulated time spent on citi bikes in 2022 than in 2021 per month, the median trip duration per month is less in 2022 than in 2021. This means that more riders are going shorter distances. In 2022, around 6-8 mins and in 2021, 8-10 mins. 
  * However, if you look deeper into this analysis, the shorter rides are similarly also coming from winter months (Sept-Dec 2021). Thus, the citi trip duration
  * Total Trip Duration (minutes) from Feb 2021 - June 2021: 4,089,758
  * Total Trip Duration (minutes) from Feb 2022 - June 2022: 4,894,626

* Citi Bike Station Popularity
  * Top Starting Station in both 2021 and 2022 was Grove St. Path.
  * The most popular stations to start or stop were similar for both 2021 and 2022 (Grove St. Path, South Waterfront Walkway- Sinatra Dr and 1st St, and Hoboken Terminal)
  * Grove St. Path citi bike station is located near the Grove Street train station and in the heart of downtown Jersey City. 
    * All citi bike stations in the dataset start in New Jersey, and none start in New York.
    * The most popular stations to start or stop a journey are also all located in New Jersey.
    * The least popular start stations are York St, JCBS Depot, and E20 St & FDR according to the data. 
    * There are several stations located in New York with a single drop-off. Citi Bike ride decision makers should consider the implications of several drop-off locations with limited riders. 

This analysis supports key findings:
* There are trends with seasonality that the city officials can take advantage of or market around to increase rides
* There are more rides in 2022 than in 2021. This could be related to COVID-19 policy implications or general growth in citi rides popularity.
* Shorter rides are more common in 2022. 
* City Stations like Grove St. Path, South Waterfront Walkway- Sinatra Dr and 1st St, and Hoboken Terminal are popular for both starting and ending a journey, and Citi bike can look into increasing bikes at these locations or ensuring there is adequate resources there for the market. 
* Similarly, there are several locations that are not popular to start including York St, JCBS Depot, and E20 St & FDR . Citi Bike should consider reducing stations at these areas or analyzing why these areas are not receiving as much traffic. 
* Citi could consider ways to incentivize riders to drop off their bike at certain locations based on this data to reduce city manpower needing to collect the bikes dispersed all around the city, especially in the several New York locations.