# New Business Opportunity Exploratory Data Analysis

# Overview 
  This project helps to decide where is the best geographical area to open a new Coffee Shop.


## Business Problem


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/USAMAP.png)


<br>
  Opening a coffee shop can be extremely profitable if you do it right. Chosing location is one of the most important step. The most central locations are not necessarily the best for business. Malls and other high-traffic locations typically have the highest rents and the most competition. Storefronts are excellent locations for coffee shops—they have the highest visibility, the rents are usually lower than in malls.
  This Project helps to make a decision on geographic location based on population of the region and average yelp rating of all coffee shops in the same region.

## Repository Structure

  All data sets can be found in `/data` folder.
  All plots and locally saved images can be found in `/PICTURES` folder.

## Analysis Focus

1. This analysis focuses on data availible from yelp search pages by requests Coffee Shops in Brooklyn and Queens.

2. This analysis focuses on demografic data by zip code from sourse: http://zipatlas.com/us/ny/zip-code-comparison/population-density.html

3. Main conclusion comes from combination of 2 factors - population per business and average rating by zip code.
   Both factors are combined into score based on weights given the importans of each factor.
   
## Analysis

### Visualization of density businesses in two boroughs - Brooklyn and Queens

  By creating map of business density we can analize where most of coffee shops located in neighborhoods. Each blue point on a map represents individual Coffee Shop. We can conclude that most of the businesses located by major commute lines and around offices and malls. 


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/DENSITY_MAP.png)<br>


The Map of business density dosn't give us clear undestanding about geografical location for new business.
Aplying math and statistical analisys to ore date we able to get more percise information about regions.
The next barchart represents amount of businessess per each borough.


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/BQ_BAR.png)<br>


Analising Bar Chart we understand that Brooklyn has more then double amount of coffee shops then Queens. 
Oure next move will be to explore Qeens with less amount of businessess.

Using webscraping technique we able to get data from web about population by zip code in Quieens.
This allows us to add another factor to our analizes. It is also helps us to combine retrived data from yelp resourse about businessess 
and build next graph. Bar chart below shows us Population per Coffee Shop at each zip code in Queens. Means zip codes with highest number population have least coffee shops.


![img](https://github.com/vanitoz/nyc_mhtn_ds_120720_Project_1/blob/main/PICTURES/COUNT_BY_ZIP.png)<br>


So based on Population and Number of businesses we can make a strong assumptions at which geographical location better to open new business.
Going further with data analizes we able to create score for each zip code in region that combines population and business ratings and helps to rank the best zip codes based on the assumptions. The score is described as:



We combined 


