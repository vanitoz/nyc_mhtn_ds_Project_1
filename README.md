# New Business Opportunity Exploratory Data Analysis

# Overview 
  This project helps to decide where is the best geographical area to open a new Coffee Shop.


## Business Problem


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/USAMAP.png)


<br>
  Opening a coffee shop can be extremely profitable if you do it right. Choosing a location is one of the most important steps. The most central locations are not necessarily the best for business. Malls and other high-traffic locations typically have the highest rents and the most competition. Storefronts are excellent locations for coffee shops—they have the highest visibility, and the rents are usually lower than in malls. The aim of this project is to help make a decision on geographic location based on population of the region and average yelp rating of all coffee shops in the same region.
  
## Repository Structure

  All data sets can be found in `/data` folder.
  All plots and locally saved images can be found in `/PICTURES` folder.

## Analysis Focus

1. This analysis focuses on data available from yelp search pages by requests at Coffee Shops in Brooklyn and Queens.

2. This analysis focuses on demographic data by zip code from source: http://zipatlas.com/us/ny/zip-code-comparison/population-density.html

3. Main conclusion comes from a combination of 2 factors - population per business and average rating by zip code. Both factors are combined into score based on weights given the importance of each factor.
   
## Analysis

### Visualization of density businesses in two boroughs - Brooklyn and Queens


  Visualization of density businesses in two boroughs - Brooklyn and Queens
By creating a map of business density we can analyze where most coffee shops are located in Brooklyn and Queens. Each blue point on a map represents an individual coffee shop. We can conclude that most of the businesses are located by major commute lines and around offices and malls.


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/DENSITY_MAP.png)<br>


### Visualizing exact differences - Brooklyn and Queens.


  The map of business density doesn't give us clear understanding about geographical location for new business. Applying math and statistical analysis to more data we are able to get more precise information about the regions. The next barchart represents the amount of businesses per borough.


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/BQ_BAR.png)<br>


  Analysing the bar chart we understand that Brooklyn has more than double the amount of coffee shops then Queens. Your next move will be to explore Queens, as it has fewer businesses.


 ### Looking for Population per Coffee Shop in each zip code in Queens.
 
 
 Using web scraping techniques we are able to get data from the web about population by zip code in Queens. This allows us to add another factor to our analizes. It also helps us to combine and retrieve data from yelp resources about businesses and build the next graph. Bar chart below shows us Population per Coffee Shop at each zip code in Queens. This shows zip codes with the largest population that has the fewest coffee shops.


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/COUNT_BY_ZIP.png)<br>


  So based on population and number of businesses we can make strong assumptions of which location is better suited to open a new business.
  
  
  ## Further analyzing with a specific equation.
  
  Going further with data analyses we are able to create a score for each zip code in the region that combines population and business ratings and helps to rank the best zip codes based on the assumptions.
  
  
  ![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/FORMULA.png)<br>
  
  
  This further helps to pair down the information that adds more insight to the decision of which zip code to build a coffee shop.
  Based on a set factors - weight population =0.8 and weight rating=0.2 our scored data came up as folllowing table:
  
  ![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/BESTSCORE.png)<br>
  
  
 ## Summary
  Despite having millions of potential customers and a lot of locations to choose from our data helped us narrow down all of the many possibilities into a more narrow set of optimal spots. Our results suggest that if we were to setup a coffee shop in zip code 11368 we would have the least competition for the most potential customers. Also the average review rating of the existing coffee shops in that zip code show there is a lot of room for improvement as the zip code wide rating is only 3.5 out of 5.
  
## Presentation

https://docs.google.com/presentation/d/1uYLp9xI4ixXBdMgJkdyNImKlLVqzdyn9JjTTtsEWENY/edit#slide=id.gaad49ec1d2_0_37

## Contributors

[Guy Monahan](https://github.com/GuyMonahan)
<br>
[Ivan Zakharchuk](https://github.com/vanitoz)


