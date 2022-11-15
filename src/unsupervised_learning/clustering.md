# Clustering

- could be clustered by location, shape, and density
- can be used in compression

## K-Means

- initialize some initial centroids
  - assign data points to clusters
  - move center of cluster to the centroid of the cluster
  - repeate

### Initialization

initialization matters cuz K-means has a lot of local minimas

- random
  - problem: may choose nearby
- distance: choose the furthest point
  - problem: often choose outliers
- K-Means++: random + distance
  - far but randomly

### Choosing K

penalize complexity

## Agglomerative 

- each point is a cluster
  - merge two closest clusters
  - repeat

The tree from merging is called the dendrogram

### Cluster Distance

Different cluster distance results in different clusters

- closest two points
- furthest two points
- average of data points
- centroids of clusters

## Gaussian

similar to K-Mean but Gaussian distribution for each cluster