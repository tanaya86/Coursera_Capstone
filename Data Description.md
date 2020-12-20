## The Battle of Neighborhoods | Data Description
Data Description:
Data Link: https://en.wikipedia.org/wiki/B_postcode_area

Will use Birmingham dataset which will scrap from wikipedia. Dataset consisting of latitude and longitude, zip codes 
: https://github.com/tanaya86/Coursera_Capstone/blob/main/postcode-outcodes.csv

Foursquare API Data:
We will need data about different venues in different neighborhoods of that specific borough. In order to gain that information we will use "Foursquare" locational information.
Foursquare is a location data provider with information about all manner of venues and events within an area of interest. Such information includes venue names, locations, 
menus and even photos. As such, the foursquare location platform will be used as the sole data source since all the stated required information can be obtained through the API.

After finding the list of neighborhoods, we then connect to the Foursquare API to gather information about venues inside each and every neighborhood. 
For each neighborhood, we have chosen the radius to be 100 meter.

The data retrieved from Foursquare contained information of venues within a specified distance of the longitude and latitude of the postcodes. 
The information obtained per venue as follows:

1. Neighborhood
2. Neighborhood Latitude
3. Neighborhood Longitude
4. Venue
5. Name of the venue e.g. the name of a store or restaurant
6. Venue Latitude
7. Venue Longitude
8. Venue Category
