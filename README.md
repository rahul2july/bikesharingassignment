# Project Name: Bike Sharing Assignment -

Problem Statement:
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system. A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.  In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits. They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends.

Requirement:
Which variables are significant in predicting the demand for shared bike
How well those variables describe the bike demands.

What we need to do: 
Create a linear model that describe the effect of various features on demand
The model should be interpretable so that the management can understand it


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

Problem Statement:
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system. A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.  In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits. They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends.

Requirement:
Which variables are significant in predicting the demand for shared bike
How well those variables describe the bike demands.

What we need to do: 
Create a linear model that describe the effect of various features on demand
The model should be interpretable so that the management can understand it

Dataset:

day.csv has the following fields:
- instant: record index
- dteday : date
- season : season (1:spring, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2018, 1:2019)
- mnth : month ( 1 to 12)
- holiday : wheather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
+ weathersit : 
    - 1: Clear, Few clouds, Partly cloudy, Partly cloudy
    - 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
    - 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
    - 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : temperature in Celsius
- atemp: feeling temperature in Celsius
- hum: humidity
- windspeed: wind speed
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- python - version 3.9.13
- numpy - version 1.22.2
- pandas - version 1.4.1
- matplotlib - version 3.5.1
- seaborn - version 0.11.2
- sklearn - version 1.1.1
- statsmodels - version 0.13.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Conclusions

Equation of best fitting line would be:
cnt = 0.1350 + 0.2327 * year - 0.1072 * holiday + 0.5471 * temp - 0.1531 * windspeed + 0.0866 * summer + 0.1323 * winter + 0.0992 * sep - 0.0500 * sun -0.2892 * Light_snow_rain -0.0819 * Misty

Significant features in predicting the demand for shared bikes:
-year
-holiday
-temp
-wind speed
-season: summer
-season: winter
-month: september
-day: sunday
-weather situation: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
-weather situation: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, MistMisty



<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Acknowledgements

This project was inspired by Linear Regression Assignment as part of Data Science course.
This project was based on: https://learn.upgrad.com/course/1991/segment/16594/129672/396956/2065942


## Contact
Created by [@rahul2july] - feel free to contact me!
Contributor -Rahul Gupta


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
