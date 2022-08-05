# Ford GoBike Analysis
## by Chelagat Pauline Gechure


## Dataset

> **About Ford GoBike Bike Sharing**

Ford GoBike implemented in 2013 is a regional bike-sharing network aimed at enhancing accessible, affordable and sustainable  transportation in the San Francisco Bay Area. Lyft rebranded the San Francisco Bay Area's bike-share program from Ford GoBike to Bay Wheels in 2017 and effected the change in June 2019. 

The bikes are designed for the hilly urban environment are therefore comfortable and easy to ride. Riders both subscribers/member and customers/casual, are able to access the bikes from various stations in the city. 

Ford GoBike System Data includes information about individual rides made in a bike sharing system in the San Francisco Bay Area. The data provided [here](https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1658068876854626&usg=AOvVaw3ly7YsFLadhywo24nm_p_8) covers February 2019. The desire is to focus on a complete year(January 2019 - December 2019) and the files can be downoaded from [here](https://www.lyft.com/bikes/bay-wheels/system-data).

> **Column mapping:**

- duration_sec
- start_time
- end_time
- start_station_id
- start_station_name
- start_station_latitude
- start_station_longitude
- end_station_id
- end_station_name
- end_station_latitude
- end_station_longitude
- bike_id
- user_type
- member_birth_year
- member_gender
- bike_share_for_all_trip

> **Data Wrangling:**

The entire 2019 dataset was downloaded and assessed programmatically. Columns with missing data were dirpped as they were not relevant for the analysis. Errenous data types were fized accordingly and relevant information such as month, date, day of the week and hour were retrieved from the `start_time` column as it was relevant for the analysis and visualization. The `duration_sec` column was converted to `duration_min` which is more conventional for communicating time.

## Summary of Findings

- Upto 80% of the users are subscribers and roughly 20% of the users are customers. March, April, July, August, September, October are the top 6 months with the highest number of bikes rides. Of importance to note, July through October coincide with summer and autumn which are characterized by warm sunny days and clear nights conducive for tourism. There are more subscriber bike rides compared to customers across the months but trend is generally the same  between the two user types with the exception of December which has almost similar number of rides between the two groups. Most subscribers take rides during weekdays with a significant drop during the weekend while customer rides are steady throughout the week. Hourly bike rides has a bimodal distribution with peaks during morning and evening hours. 

- Generaly, bike ride duration is skewed to the right with most trips taking 30 minutes. Customers have average bike rides being twice as long as the average subscriber bike ride.Over the months, customers had a higher average bike ride duration compared to subscribers. There was a steady marginal decline in the average bike ride duration for customers compared to subscribes who had a stable average throughout the year. December also had a marginal difference between customer and subscriber bike ride duration. Bike ride durations peaked between June and October 2019 and drop as the year came to a close. Most subscribers use bike during weekdays with the rides lasting between 5 and 20 minutes. Customers on the other hand use the bikes throughout with slightly hihger average bike ride durations of between 10 and 30 minutes. Most trips were take between 7am and 8am and 4pm and 6pm which coincide with commute hours.


## Key Insights for Presentation
- Upto 80% of the users are subscribers and consequently more bike rides from them.
- Customers have average bike rides being twice as long as the average subscriber bike ride.
- Most subscriber rides happen during the weekdays with a drop during the weekend but there is a steady demand for the bikes from customers throughout.
- Bike ride durations peaked between June and October 2019 and drop as the year came to a close.
- Most bike rides happen during morning hours between 7am and 8am and evening between 4pm and 6pm.