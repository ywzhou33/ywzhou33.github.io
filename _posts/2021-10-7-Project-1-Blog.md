ST 558 Project 1
================
Aries Zhou
10/07/2021

#### Project 1 Backgrounds

This Project is to access data sets from the One Call API and perform
data exploration and graphical summaries.

Connects to the One Call API.

The One Call API provides the following weather data for any
geographical coordinates:

  - Current weather  
  - Minute forecast for 1 hour  
  - Hourly forecast for 48 hours  
  - Daily forecast for 7 days  
  - National weather alerts  
  - Historical weather data for the previous 5 days

These data can be accessed by defining parameters in the URL. I selected
84 data sets by longitudes across the latitude 35.78 (each data is 4.3
longitudes away from each other with the same latitude). I choose a
latitude of 35.78 because this is where NC State is located. These small
data sets each containing 8 observations of current and future 7 days
weather forecasting information are then selected and recombined into a
full data set.

New variables of Wind Status and Area are created and the average daily
temperature is calculated for further data summaries.

The following graphs are used to compare the differences between the
land and water/ocean areas across the latitude of 35.78 on Earth.

  - Histogram for Temperature
  - Boxplot for Temperature
  - Barchart for Wind Status
  - Boxplot for Humidity
  - Scatterplot for Wind Status v.s. Humidity.

#### Findings

  - Wind status on the land area is more calm while it is more windy
    over the water area.  
  - The water area tend to have higher average daily temperature in the
    future 7 days. This is a little surprising since I was expecting
    windy areas to be cooler.  
  - While both of the temperature and humidity over the water areas are
    higher in general, the temperature and humidity varies more on the
    land areas.  
  - There is a slight positive correlation relationship between the
    temperature and humidity. Warm air tend to hold more vapor than cool
    air.

#### Reflections

The most difficult part of the logic and programming Initially, the most
difficult part for me is to choose data from the APIs. The massive and
diverse data options are overwhelming. For the logic and programming,
the data manipulation section was the most difficult part. The datasets
from the API came with a complicate structure, which enhanced the
difficulty to manipulate them in the wrapper function.

In the future project, I will try to improve the function efficiency in
approching the results, such as using the repetition function, lapply or
parallel computing instead of for loops.

#### [Link](https://github.com/ywzhou33/ST558-Project-1.git) to the Github Pages repo and [link](https://github.com/ywzhou33/ywzhou33.github.io.git) to Github Blog repo.
