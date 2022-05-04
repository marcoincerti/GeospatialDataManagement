# Clustering
We have data about the historical stores and bus stops in Milan.
We want to help the municipality to support and manage the shopping activities in the city by:
* Determine the shopping areas: the areas where the stores are dense.
* Determine if these areas are well served by public transport. An area is considered well served by transportations if there are in average at least 10 bus stops for each 1km.

##Procedure:
* Apply DBSCAN on the stores data in order to detect the dense areas. We can represent each dense area by a polygon.
* We need to find how many bus stops exist in each shopping area=> find the intersection between the bus stops (represented as points) and the shopping areas (represented as polygons)
* Check if the number of bus stops is enough in each area according to its surface.
