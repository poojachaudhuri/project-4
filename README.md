# 311 complaints related to heat and hot water

This project analyses 311 service requests related to heat and hot water from NYC Open Data. The time period for the data is 2020 to 2022. It explores the complaints on the borough level, zip code level, and traces the building which has an outsized number of complaints. The data has been normalized by the zip code level population data gathered from U.S. Census Bureau. The result is this story - [Bronx leads city in heat and hot water complaints. One building has an outsized share of complaints.](https://poojachaudhuri.github.io/project-4/)

## Guide to the repository ##

 `notebooks:` This folder contains all the python notebook. `cleaning.ipynb` contains the code that was used to clean the 311 data. `census.ipynb` contain all the code to make API calls to the U.S. Census Bureau data. The API was used to get data related to zip code level population, median income and percentage below poverty. `zip_codes.ipynb` contains the code that was used to scrape [nycnatives.com](https://www.nycbynatives.com/nyc_info/new_york_city_zip_codes.php) which has a list of NYC zip codes. `plotting.ipynb` contains R (ggplot2) codes used to plot the data and make charts that were later cleaned on Adobe Illustrator. 
 
 `docs:` This folder contains the parquet and csv files for the 311 data, census data and zip codes. 
 
 `images:` Contains all the images of the charts used in the html file. The images were generated using ai2html. 

## Findings ##

An analysis of the data revealed that the Bronx has the highest number of complaints boroughs in all the three years. In 2022, Bronx accounted for more than a third of the total complaints. Out of the top 10 addresses with the highest number of complaints in 2022, seven were in the Bronx. However, one address in Northwest Bronx - 2176 Tiebout Avenue - had a vastly outsized share, with over 3,000 complaints. This address accounts for a third of all the complaints from the Bronx zip code 10457. 

## Limitations ##

311 data may not give a picture of the ground reality. To infer that a certain zip code which has more complaints also has more violations related to heat and hot water can be misleading. There may be households that are not complaining despite facing issues, or some households may be complaining a lot of more than others. After speaking with a few residents of 2176 Tiebout Avenue, I found that the building has only 20 apartments. Over 3,000 complaints from a single building in a single years hints to the fact that there are households making multiple complaints. 311 data is not recorded at the apartment address level but building address level. 

Further ground reporting - which means talking to every resident of 2176 Tiebout Avenue - would give a clearer picture about the inflated number. 

