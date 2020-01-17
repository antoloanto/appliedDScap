## NEIGHBOROHOOD COMPARISON USING FOURSQUARE - TORONTO AND NEW YORK

### Index
1. Business Problem
2. Data Gathering and Organization
3. Data Analysis
4. Machine Learning
5. Results
6. Conclusion

### Index
- Installing and importing
- Data Gathering and Organization
    1. NYC Manhattan Data
    2. Toronto Data
    3. NYC Demograph
    4. Toronto Demograph
    5. FourSquare
        - Start Manhattan NYC
        - Start Toronto
- Data Analysis
    1. NYC Manhattan neighbourhood
    2. Toronto Downtown neighbourhood
- Machine Learning
    1. k-means to cluster the NYC Manhattan neighborhood
    2. k-means to cluster the Toronto Downtown neighborhood
- Results
    1. NYC Manhattan
    2. Toronto Downtown

### 1 Business Problem
*"That's Food"*, an international company with many reasturant in many country of the world, want to open a new restaurant in the North America. After several board meeting they decided that the two cities to consider are  New York and Toronto, but doesn't know which one of these two neighbourhoods, the Manhattan and the Downtown in the New York City and the Toronto City respectively, is better to open or site a company or business. Hence they decided to hire a team of data scientist to solve the problem to choose the right neighbourhood for *"That's Food"* to open a new restaurant.  

###### The right audience for this work is the *"That's Food"* management .
######## The aim of the project is understand what is the best city and his neighbourhood to be considered for opening a new restaurant.

### 2 Data Gathering and Organization     
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

--- INSERT LINK --- See the code [Here](...) at the DATA GATHERING AND ORGANIZATION point --- INSERT LINK ---
      
### 3 Data Analysis
The data sets of the two neighbourhoods, Toronto Downtown and the Manhattan were visualized to gain knowledge of the distribution of variables and the neighbourhoods in the Boroughs, using folium library. Later it was checked how much these data are correlated.

--- INSERT LINK --- See the code [Here](...) at the DATA ANALYSIS - NYC Manhattan and the Toronto Downtown point --- INSERT LINK ---

### 4 Machine Learning
Here the encoded data during the analysis are fed into the machine learning algorithm - K-mean Clustering - to group or segment the neighbourhoods. At the end, the neighbourhoods that have similar characteristics are grouped together. Thence the similarities and dissimilarities of the Downtown and the Manhattan are observed.

--- INSERT LINK --- See the code [Here](...) at the MACHINE LEARNING - NYC Manhattan and the Toronto Downtown point --- INSERT LINK ---
### 5 Results
- See the image1 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)
- See the image2 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)
- See the image3 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)
- See the image4 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)
- See the image5 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)
- See the image6 [Here](https://github.com/antoloanto/appliedDScap/blob/master/week5source/1)

### 6 Conclusion
The neighborhoods are similar when one considers only the question of the location of the restaurant.
The difference to focus on is the issue of population density, which is much greater in NYC.
Therefore, it will be better to open the new *"That's Food"* restaurant in Manhattan to earn more money.
