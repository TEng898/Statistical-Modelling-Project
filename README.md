# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
This purpose of this project is to determine if relationships exists between the number of city bikes available at the various locations (stations) and any of the points of interests in the city of Vancouver, BC. The Yelp and Foursquare APIs were used to retrieve the data using python. The data was analyzed using the pandas package and modeled using the statsmodels package.

## Process
### 1. Send requests to the Yelp and Foursquare APIs for points of interest (POI).
### 2. Parse the returned data using python and import into pandas data frames.
### 3. Apply EDA process to explore the data using visualizations. Check for any relationships.
### 4. Export all data into SQLite database and verify integrity of data
### 5. Model the number of city bikes and various POI using the statsmodels package for statistical significance of relationships. 

## Results
The Yelp API provided more complete data. It gives ratings and the number of ratings of points of interest (POI) which were not available in the Foursquare API. The Foursquare V3 API also has a limitation of 50 POIs per API call so the amountof data is limited. The Yelp API is also limited by 50 POI per API call but it also offers an offset parameter that allows retrieval of more results. However, the Foursquare V2 API allows for retrieval of up to 100 POIs per API call along with the offset parameter to retrieve more results.

## Challenges 
Trying to find categories of POI that were general enough to classify them into specific groups were a challenge since the returned data were often too specific. For example, Ramen noodles or Sushi were returned instead of restaurant.
Trying to find relationships between the number of city bikes available at various stations and POIs were also challenging as there are not many with significant relationships.
## Future Goals
Explore the more various POIs to see if stronger statistical relationships exists with the number of city bikes. Change the radius of the search for more granular filtering of nearby POIs.