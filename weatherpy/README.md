# python-api-challenge
WeatherPy Assignment

1) generated random list of cities from CityPy.
2) Used the city list to pull the following information about each city from WeatherPy into a data frame called city_df
a) latitude
b) longitude
c) maximum humidity
d) cloudiness
e) wind speed
f) country, and 
f) date
3) set the above query up to generate a data retrieval log
4) used the describe function to provide an overview of the data in the city_df
5) determined that there were no cities selected with humidity > 100
6) evaluated humidity data for outliers
7) reran the describe function after eliminating humidity outliers
8) created the following scatter plot charts and commented on the results of each scatter chart.
a) Latitude vs. Max Temperature
b) Latitude vs. Humidity
c) Latitude vs.Cloudiness
d) Latitude vs. wind speed
9) segregated the above data into Northern and Southern Hemisphere and performed the following for each hemisphere
a) ran the describe function after eliminating humidity outliers
b) created the following scatter plot charts and commented on the results of each scatter chart.
b1) Latitude vs. Max Temperature
b2) Latitude vs. Humidity
b3) Latitude vs.Cloudiness
b4) Latitude vs. wind speed
10) downloaded cities_df to a .csv file to the output folder for use in the VacationPy assignment
11) save a png copy of all scatter plot charts created for this assignment to the output folder

WeatherPy Observations

Looking at the sample selected, as a whole after removing outliers, the average maximum temperature was approximately 48 degrees Fahrenheit with a comparatively high standard deviation of approximately 35 degrees which indicates that the average is really not representative of the sample.  Given how broad this sample was across latitudes this really is not surprising.

Overall, temperatures have a stronger correlation to latitude while cloudiness, humidity and wind speed really did not have much of a correlation.  

When breaking down the data by hemisphere, in the Northern Hemisphere, the average temperature is approximately 35 degrees with still a very large standard deviation of 36 degrees. 

In the Southern Hemisphere, the average temperature is approximately 73 degrees with a standard deviation of 10 degrees, which would indicate that the mean in the Southern Hemisphere is much more representative than in the Northern Hemisphere.  

In the Northern Hemisphere there is a negative correlation and linear regression as latitude increases. 

In the Southern Hemisphere, there is a positive correlation and linear regression as latitude increases.  

For both hemispheres the respective samples show a clear relationship between weather and latitude but very little relationship between latitude and humidity, cloudiness and wind speed.  

VacationPy Assignment

1) Imported the cities.csv (formerly cities_df)
2) using gmaps, created a heatmap of the data in in the cities.csv
3) created a new DataFrame named weather_df that filtered the cities based on the following:
a) maximum temperature >70 degrees and <80 degrees
b) wind speed < 10 mph
c) cloudiness = to 0
4) using the latitude and longitude coordinates from the filtered weather_df, pulled in hotel data into a list called places_data from Google Places
5) created a DataFrame named hotel_df with the following data from the first listing at each location in the places_data list
a) hotel name
b) latitude
c)longitude
d) place ID
6) pulled city and country into the hotel_df DataFrame from Google Place Details using the place ID in the hotel_df
7) created a marker layer and placed it on top of the previously created heat layer map.  
8) saved copies of the heat layer map created in item 2 and the marker layer map created in item 7 and saved them to the output folder
