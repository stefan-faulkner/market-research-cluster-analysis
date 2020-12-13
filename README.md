# Market Research Cluster Analysis

**Data Summary**
- Column A is the ID
- Column B is a constant, and we ignore that
- Read in columns that start with an E_ for clustering

## PART A
### Given approach
- Factor analysis with a quartermax rotation
- Metric of factors if eigenvalue is >1
- k-means clustering on the factor scores
- Clustering all 400 based on the four factors (not sure if it's actually 4) --> Number of factors based on eigenvalue greater than 1, not har coded as 4
- k is 2-6 clusters

### Open-ended approach
- Interested in using a Pearson distance measure.  Has to be coded in
- <a href="https://scikit-learn-extra.readthedocs.io/en/latest/user_guide.html#k-medoids">k-medoids</a> could be good because it works for any distance measure
- cosine distance measure
- Auto-SKLearn - iterates through multiple methods

### Two methods to identify optimal clusters
- Mean square distance
- Screeplot/elbow plot


## PART B
Now that everyone is clustered, what best predicts the clusters?

Classification with decision tree or random forest

Another thought is to use strategic binning to "re-scale" the data and use it to classify the clusters
