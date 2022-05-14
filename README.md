# World_Weather_Analysis and WeatherPy
## Overview of Project
### A travel agency needs to develop an application where clients can find the best travel locations in the globe at any given time of the year. The input client's provide is minimum and maximum temperatures for their ideal vacation. 
### Process to Retrieve the Weather Data
#### Using OpenWeatherMap API, hundreds of cities near randomly generated latitudes and longitudes were gathered. The current weather data was collected and presented into a dataframe for all cities in various countries. See the below snippet of the dataframe.
Weather Data for 5/14/2022
![image](https://user-images.githubusercontent.com/102757676/168451202-b0b1e36e-5249-4720-b444-20f8d68e9065.png)

### Creating the Customer Travel Destinations Map of Possibilities
#### The dataframe retrieved was filtered by client input of minimum and maximum temperature range for their ideal vacation locations. A new dataframe was created with the filtered results and the closest hotels to each city center were added to the dataframe. Using the Google Maps API, a map of all acceptable locations based on current teamperature was generated. On top of the map, markers were added to designate the hotels in each of the cities. Pop-up information was added so that when markers are selected, the Hotel Name, City, Country, and Current Weather conditions plus the day's Max Temperature is displayed. See the below example.
Vacation Search Map

![image](https://user-images.githubusercontent.com/102757676/168451221-54dbd614-83e6-4615-a37c-b51acbedc6f7.png)

### Creating a Travel Itinerary Map
#### The map acceptable cities was used to select four cities within one country for the client to visit. Using the to_numpy() function and list indexing, the latitudes and longitudes of each city were extracted into a tuple. These tuples containing the cities' latitudes and longitudes were used with the gmaps directions layer added ontop of the gmaps figure with markers denoting the individual city destination points. See below figure.

Vacation Itinerary Driving Directions

![image](https://user-images.githubusercontent.com/102757676/168451377-e6e34969-59fb-444f-bf54-c9f930ca9f1f.png)


#### Finally, the pop-ups were added to the map and the driving directions removed. The final map provides the hotel name, city, country, and current weather data for each of the four cities the client will visit on their vacation. See below figure.

Vacation Itinerary Hotels and Current Weather

![image](https://user-images.githubusercontent.com/102757676/168451379-fc313e2d-ac84-4429-a224-5301e15cab5b.png)
