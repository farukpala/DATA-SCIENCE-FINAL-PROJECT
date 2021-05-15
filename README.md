
# Battle of Neighborhoods-The Smart Investor 
## Finding the best neighborhood of Istanbul to invest in Fastfood


## A.Introduction

### A.1.Business Problem

Imagine that ,You are an investor who want invest into profitable businesses on all around the world. You have the capital and want to invest in Turkey.There are many options on the desk .

**Invest in a fast food restaurant in Istanbul ?**

If we ask this question without using our data science powers , it sounds quite bare and meaningless.
Turkey’s fast food market size 2.4 billion dollars and it continues to grow.The word of “2.4 billion dollars market size“ Things are getting heating up.
The financial health and stability the sector is strong and getting stronger. Increasingly , Turkey’s young population promises a high potential on fast food sector.
Aim of this project is to find optimal locations to open franchise fast food restaurants.Especially , This report will be targeted to guide investors who wants to invest in fast food restaurant in Istanbul.
Istanbul is the 14th most populated metropolis of the world with its 15 million people, 38 borough and 968 neighborhood. Therefore, a little question comes into my mind,
Which part of Istanbul we should invest ?
My aim is to detect neighborhoods that have less rivals and have most potential customers.
Now , Lets’s dive into data ocean to find optimal answers.

### A.2. Data Description

I built my project on 2 main factors,

** a.I focused on percentage of fast food restaurants on all food venues.I categorized venues into 4 groups include fast food and venues which can be alternative to fast food restaurants. ([venue_categories.csv](https://github.com/farukpala/DATA-SCIENCE-FINAL-PROJECT/blob/c7dd0da874bb801f938f574738113f748405254d/venue_categories.csv))

*  Fast Food

*  Restaurants

*  Cafe (includes cafe’s and bars )

*  Dessert shops

** b.I focused on age -fast food consumption correlation, People between 15–35 age group are my target customers;

a. According to a statistical hypotesis, age and fast food consumption have strong correlation.( provided by “Ekev Academic Magazine”)
b. In addition , According to a survey about fast food habits in Turkey , 45% of fast food consumers were aged 16–34 ( provided by “Mediabrands/Insight Research Company” )


1.Second-level Administrative Divisions of the Turkey json file to create coropleth map via ratio of potential customers.(Provided by Spatial Data Repository of NYU )([json file](https://github.com/farukpala/DATA-SCIENCE-FINAL-PROJECT/blob/ab2a8f37845efcdb2a7739e121259385e83bc5d1/stanford-nj696zj1674-geojson.json)) [1]

2.**Foursquare api**  to detect food venues in neighborhoods[2] 

3.Turkish Statistical Institute , Medas platform –Demographic data of Istanbul boroughs to detect age and population distribution ([istanbul_demographic.csv](https://github.com/farukpala/DATA-SCIENCE-FINAL-PROJECT/blob/ab2a8f37845efcdb2a7739e121259385e83bc5d1/istanbul_demographic.csv))[3] 

4.Geocoder Library to detect coordinates of neighborhoods  


5.İstanbul Metropolitan Municipality open data portal to detect neighborhood populations ([neighborhood_pop.csv](https://github.com/farukpala/DATA-SCIENCE-FINAL-PROJECT/blob/292f97dbd809eb0e67bf35eb970af63c20168d98/neighborhood_pop.csv)) [4]

6.Google Map, to get the  coordinates of the each borough. ([istanbul_geo.csv](https://github.com/Srcanyildiz/istanbul/blob/master/istanbul_geo.csv)) [5].

7.Foursquare api lets 800 request per day , So I deleted some neighborhoods from 963 to 798 and saved as ([neighborhood_coordinates.csv](https://github.com/farukpala/DATA-SCIENCE-FINAL-PROJECT/blob/8186d18f38017b7455bb331ce5a3dd1b02a0bdc3/neighborhood_coordinates.csv)) Query takes nearly 30 minutes

## References

[1] [Second-level Administrative Divisions of the Turkey](https://geo.nyu.edu/catalog/stanford-nj696zj1674)

[2][Foursquare API](https://developer.foursquare.com/)

[3][Medas Platform](https://biruni.tuik.gov.tr/medas/?kn=95&locale=tr)

[4][Neighborhood populations](https://en.wikipedia.org/wiki/Istanbul)

[5][Google Map](https://www.google.com/maps/)


