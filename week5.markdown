## Neighborohood Comparison Using FourSquare - NYC Manhattan and Toronto Downtown

### Index
1. INTRODUCTION to Business Problem
    - Installing and importing
2. DATA Gathering and Organization
    - Examples and link to code 
3. METHODOLOGY
    1. Data Analysis
        - Examples and link to code 
    2. Machine Learning
        - Examples and link to code 
4. RESULTS
5. DISCUSSION
6. CONCLUSION

---

### 1 INTRODUCTION to Business Problem
*"That's Food"*, an international company with many reasturant in many country of the world, want to open a new restaurant in the North America. After several board meeting they decided that the two cities to consider are  New York and Toronto, but doesn't know which one of these two neighbourhoods, the Manhattan and the Downtown in the New York City and the Toronto City respectively, is better to open or site a company or business. Hence they decided to hire a team of data scientist to solve the problem to choose the right neighbourhood for *"That's Food"* to open a new restaurant.  

The right audience for this work is the *"That's Food"* management .
The aim of the project is understand what is the best city and his neighbourhood to be considered for opening a new restaurant.

###### - Installing and importing
First of all it is necessary to install the geopy and folium libraries in order to carry out the project.

- Geopy : Find the coordinates of addresses, cities, countries and landmarks around the world using third-party geocoders and other data sources.
- Folium : display spatial data (all data types that contain geographic data types such as latitude and longitude) and generate insights

Other Libraries :
- Numpy         : handle data in a vectorized manner
- Pandas        : high-performance, easy-to-use data structures and data analysis tools
- Matplotlib    : 2D plotting library which produces publication quality figures in a variety of hardcopy formats
- k-means       : from clustering stage
- Beautifulsoup : to scrape the data from the web
- json          : to handle JSON files

### 2 DATA Gathering and Organization     
Datasets :

- Demographics of New York City from - [NYC Open Data](https://opendata.cityofnewyork.us/)
- Demographics of New York City from wikipedia - [Demographics of New York City](https://en.wikipedia.org/wiki/Demographics_of_New_York_City)
- Demographics of Toronto Neighbourhoods from wikipedia - [Demographics of Toronto Neighbourhoods](https://en.wikipedia.org/wiki/Demographics_of_Toronto) and [Demographics of Toronto Neighbourhoods](https://en.wikipedia.org/wiki/Demographics_of_Toronto_neighbourhoods)
- List of Postal Codes of Canada from wikipedia - [Canada List Postal Code](https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M)
- Boroughs of Nework City from wikipedia - [Boroughs of New York City](https://en.wikipedia.org/wiki/Boroughs_of_New_York_City)
- Foursquare API Geolocation data - [Foursquare API](https://it.foursquare.com/)

The attributes of the data are:

- identity numbers
- longitudes
- latitudes
- boroughs
- neighbourhoods
- venue
- categories
- population
- average income
- gdp (gross domestic product)
- tips
- etc

The identity numbers are the numbers that uniquely identify the tuple. Latitude and Longitude are the geographic coordinates 
and are respectively the numeric line running east and west of the earth and the imaginary line running north and south of Green Wich meridian. The borough is a subset of a city. The neighbourhood is the community area name.

The target value (variable) or label of the data set is the neighbourhood which is the dependent variable. The other variables is like longitudes, latitudes, venues, etc are the independent (predictor) variables.

###### - Examples and link to code
Example of data collected for NYC Manhattan : 
- [NYC Data](https://github.com/antoloanto/appliedDScap/blob/master/week5source/0-data.JPG)
- [NYC Demographs](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1-demograph.JPG)
- [NYC Venues](https://github.com/antoloanto/appliedDScap/blob/master/week5source/3-venues.JPG)

See the code [Here](https://github.com/antoloanto/appliedDScap/blob/master/AppliedDS_Capstone-BattleofNeighborhoods.ipynb) at the DATA GATHERING AND ORGANIZATION point
      
### 3 METHODOLOGY
### 3.1 Data Analysis
The data sets of the two neighbourhoods, Toronto Downtown and the Manhattan were visualized to gain knowledge of the distribution of variables and the neighbourhoods in the Boroughs, using folium library. Later it was checked how much these data are correlated.

###### - Examples and link to code
Example of most common venues for NYC Manhattan and Toronto Downtown : 
- [NYC Most Common Venues](https://github.com/antoloanto/appliedDScap/blob/master/week5source/4-nyc-common.JPG)
- [Toronto Most Common Venues](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1-Toronto-common.JPG)

See the code [Here](https://github.com/antoloanto/appliedDScap/blob/master/AppliedDS_Capstone-BattleofNeighborhoods.ipynb) at the DATA ANALYSIS - NYC Manhattan and the Toronto Downtown point

### 3.2 Machine Learning
Here the encoded data during the analysis are fed into the machine learning algorithm - K-mean Clustering - to group or segment the neighbourhoods. At the end, the neighbourhoods that have similar characteristics are grouped together. Thence the similarities and dissimilarities of the Downtown and the Manhattan are observed.

###### - Examples and link to code
Example of most common venues for NYC Manhattan and Toronto Downtown : 
- [NYC Cluster 1 example](https://github.com/antoloanto/appliedDScap/blob/master/week5source/5-nyc-cl.JPG)
- [Toronto Cluster 1 example](https://github.com/antoloanto/appliedDScap/blob/master/week5source/2-toronto-clus.JPG)

See the code [Here](https://github.com/antoloanto/appliedDScap/blob/master/AppliedDS_Capstone-BattleofNeighborhoods.ipynb) at the MACHINE LEARNING - NYC Manhattan and the Toronto Downtown point
### 4 Results
- NYC venues number [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/7-num-venus.JPG)
- Toronto venues number [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/4-venues-list.JPG)
- NYC venues map [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/6-nyc-map.JPG)
- Toronto venues map [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/3-toronto-map.JPG)
- NYC clusters map [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/8-nyc-map2.JPG)
- Toronto clusters map [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/5-toronto-map2.JPG)

See the code [Here](https://github.com/antoloanto/appliedDScap/blob/master/AppliedDS_Capstone-BattleofNeighborhoods.ipynb) at the RESULTS point

### 5 Discussion
The neighborhoods are similar if considers banks, markets, college. This venues represents availability of capital and presence of people. It is important not only the question of the location of the restaurant. 
The difference to focus on is the issue of population density, which is much greater in NYC.

### 6 Conclusion
Therefore, it will be better to open the new *"That's Food"* restaurant in Manhattan to earn more money.

---
