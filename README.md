# web-scraping-decathlon

The project is about web scraping information on Decathlon stores in various cities in India and extracting relevant data from each store's webpage. The extracted data includes the store name, address, contact number, opening hours, and latitude and longitude coordinates.

The project uses several libraries and modules, such as requests, pandas, Beautiful Soup, re, and geopy. Requests is used to send HTTP requests to the webpage, pandas is used for data manipulation and analysis, Beautiful Soup is used to extract relevant data from the HTML code, re is used for regular expression matching, and geopy is used for geocoding (i.e., converting addresses into latitude and longitude coordinates).

The code loops through a list of Decathlon store URLs and uses Beautiful Soup to extract relevant information from each store's webpage. The code then processes the extracted information to extract the relevant data (name, address, etc.), and uses geocoding to convert the address into latitude and longitude coordinates. The resulting data is stored in a pandas DataFrame and exported to a CSV file.

Overall, the project appears to be a useful exercise in web scraping and data extraction, and could be helpful for anyone looking to gather information on Decathlon stores in India.

For collecting data from a retail store I searched many retail store’s websites for finding which website contains all the data. At last I came to see the Decathlon website, in that the data are distributed over different pages so that to scrap all the data together I individually copied all links and created a list and then start scrapping . For getting latitude and longitude of places there is a need for API key but instead of that I used another technique I used Nominatim library , And then used regex library to extract pin code from address and with the radius I find the latitude and longitude. As in some address there is no pin code so in that row there is no coordinates also.
