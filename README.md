#  Capstone Project - The Battle Of Neighborhoods - Finding Better Place in Cheap Price for opening a restaurant

## Introduction: Business Problem

Birmingham is a major city in England’s West Midlands region, with multiple Industrial Revolution-era landmarks that speak to its 18th-century history as a manufacturing powerhouse.

In this project we will try to find an optimal location for a restaurant. Specifically, this report will be targeted to stakeholders interested in opening a **Restaurant** in **Birmingham**, England, United Kingdom.

Since there are lots of restaurants in Birmingham we will try to detect **locations that are not already crowded with restaurants**. We are also particularly interested in **areas with no restaurants in vicinity**. We would also prefer locations **as close to city center as possible**, assuming that first two conditions are met.

We will use our data science powers to generate a few most promissing neighborhoods based on this criteria. Advantages of each area will then be clearly expressed so that best possible final location can be chosen by stakeholders.

## Data

Based on definition of our problem, factors that will influence our decission are:
* number of existing restaurants in the neighborhood (any type of restaurant)
We decided to use regularly spaced grid of locations, to define our neighborhoods.

Following data sources will be needed to extract/generate the required information:
* Neighborhoods will be generated algorithmically and approximate addresses of boroughs  will be obtained using **https://en.wikipedia.org/wiki/B_postcode_area**
* number of restaurants and their type and location in every neighborhood will be obtained using **Foursquare API**
* coordinate of Birmingham  will be obtained using **CSV File:postcode-outcodes.csv**.

## Methodology

In this project we will direct our efforts on detecting areas of Birmingham that have low restaurant density, particularly those with low number of Indian restaurants. We will limit our analysis to area ~500m.

In first step we have collected the required **data: location and type (category) of every restaurant within 500m from Birmingham** . 

Second step in our analysis will be focus on most promising areas and within those create **clusters of locations that meet some basic requirements** established in discussion with stakeholders: we will create clusters (using **k-means clustering**) of those locations to identify general zones / neighborhoods / addresses which should be a starting point for final 'street level' exploration and search for optimal venue location by stakeholders.

## Result

Map Of Birmingham

![alt](https://github.com/tanaya86/Coursera_Capstone/blob/main/Map%201.JPG)

Value Of K By Elbow Method

![alt](https://github.com/tanaya86/Coursera_Capstone/blob/main/Cluster.JPG)

Map Of Birmingham With Top Venues

![alt](https://github.com/tanaya86/Coursera_Capstone/blob/main/Map%202.JPG)

## Discussion

The major purpose of this project, is to suggest a better neighborhood in a new city for the person who wants to open a new restaurant. Social presence in society in terms of like minded people. Connectivity to the airport, bus stand, city center, markets and other daily needs things nearby.

* Sorted list of house in terms of housing prices in a ascending or descending order

## Conclusion

Purpose of this project was to identify Birmingham areas with low number of restaurants in order to aid stakeholders in narrowing down the search for optimal location for a  restaurant.Clustering of those locations was then performed in order to create major zones of interest (containing greatest number of potential locations) and addresses of those zone centers were created to be used as starting points for final exploration by stakeholders.

Final decission on optimal restaurant location will be made by stakeholders based on specific characteristics of neighborhoods and locations in every recommended zone, taking into consideration additional factors like attractiveness of each location (proximity to park or water), levels of noise / proximity to major roads, real estate availability, prices, social and economic dynamics of every neighborhood etc.
