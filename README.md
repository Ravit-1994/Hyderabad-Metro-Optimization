# Hyderabad-Metro-Optimization

I have been travelling with my wife in metro for the past 3 weeks regularly and looking at the traffic along with the occupancy of metros wanted to understand if there were any operational issues that could be fixed.

Downloaded the Open data available and started analysis in *Jupyter Notebooks* using **Python**.

The file had .txt data containing: 
#### 'agency', 'calendar', 'fare_attributes', 'fare_rules', 'routes', 'stop_times', 'stops' and 'trips'

- agency contains the data related to the authority handling the services of the Metro.
- calendar contains the data of the trips either completed or not during a given week with the start data and end dates.
- fare_attributes has the price related information.
- fare_rules has the origin and destination with the fare info.
- routes has the color coded info and the network.
- stop_times has timestamp related information for each stop along the routes.
- stops has the longitudinal and latidudinal info of the stops and the platform numbers as well.
- trips has the directional information.

## Analysis was conducted for the geographical distribution of stops, time intervals between trips, number of trips per day and part of the day.
### Insights:
1) The consistency during Weekdays for number of trips is maintained but is far less compared to Saturday.
2) The BLUE dots indicate Hub points or Transfer Junctions along the network which are mainly spread across 3 different routes.
3) There is an even distribution of stops number along the network indicating good coverage of the city.
4) The Average interval between trips is at the highest during Morning and is lowest at Evening which could be to the overcrowding.
5) The highest trips are conducted during Mid-day i.e., between 10 AM to 4 PM then gradually it decreases.

#### Based on hypothetical scenarios where the occupancy is the highest during the morning peak and the number of passengers is constant, adjusted the number of trips to optimize the operations.

Increased the values for both Peaks by 20% and reduced the other times by 10% to find a better balance between service satisfaction and handling overcrowding.
