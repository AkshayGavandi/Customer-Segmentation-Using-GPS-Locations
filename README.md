</h2>Customer Segmentation using Location History</h2>

Abstract
Sales and Marketing Directors never have a confident answer to the question:
“How do I get my products and services in front of right people at right time?”

The key to this answer is using Customer Segmentation. It is one of the best market research strategy that helps the business find the right customer group to target. The aim of this project is to extract location information from a customer and find its characteristics based on it. This improves the convenience of the customer in accessing services and in long run benefits the companies as their target customers are focused groups which means effective usage of resources.

Data Source
The dataset includes our own location history and collections from roommates and friends. 
The datasets were downloaded from https://takeout.google.com/settings/takeout
The json data files from Google Takeout contained all location data, activity, check ins of that google ID. The latitude, longitude columns are sliced to visualize the data on world map and certain targeted locations to see the customer activity.
Another important data that is required for the project is the category was taken from google place search API  https://developers.google.com/places/web-service/search





Approach
One of the ways to find the happenings of a customer is by querying his check-in history at different locations through social media and mobile apps. However, it’s not always that a person may choose check-in and share posts on social media. Also, since this project targets to enhance the categorization of the customers based their whereabouts, the dataset includes location history of all the places visited by a person. The google places search API is used to query the type of places around the locations visited by the person.

This fetches a json result for every latitude-longitude visited by the person where we pick the type of the places nearby. The combined results provide a categorical array of places visited by the person which are counted and plotted as reports of segmentation.

Data Visualization
The data for Person A in Boston area is visualized using Basemap 
 


Code snippet to extract places from locations visited by the customer
 



Results of ‘Hits’ (number of times a person visits a location) 

   







References:

Extraction of dataset from google location history using Google takeout 
https://takeout.google.com/settings/takeout

Mapping Google location history 
http://geoffboeing.com/2016/06/mapping-google-location-history-python/

Google Place Search 
https://developers.google.com/places/web-service/search

python-google-places 
https://github.com/slimkrazy/python-google-places

