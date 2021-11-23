# Customer Clustering using K-Means

## Problem: 
Categorizing the information based on Amount income by Age.

## Dataset: 
Amount spent analysis and separate data as different category.

## Explore the data: 
Load the data and see the details such numbers of rows and columns & content.

      Separate e zipping the dataset:
      Age = df['Age'].values
      Savings = df['Income'].values
      X = np.array(list(zip(Age, Savings)))

## K-Means: 

It's an algorithm for working with unsupervised learning. This is different from supervised learning, where you tell the computer what to look for and learn,
with examples containing the labels in advance. In unsupervised learning, we don't know exactly what we are trying to teach the computer. Because of this we need to resort 
to logical segmentation groupers, with a focus on finding similarity between the sample data.

The expected result is that a pattern is found and that pattern is assumed to be what we are trying to teach the computer. Once the pattern is discovered, any new item that
has a similarity to that segment in a cluster, that is, it can be inferred as “part of that”.

## Choose the best k value: Elbow method

In this method, the average distortion of the clusters must be calculated, which is the average distance from the centroid to all points in the cluster and is obtained with 
the K-Means algorithm as a function of the number of clusters. Thus, when moving from a situation where the number of clusters is less than correct to a situation where the
number is adequate, the dispersion value decreases drastically, while if the number of clusters increases to correct, the value of scatter will decrease more slowly, forming
a curve on the graph.

- Inertia (WCSS): It is the sum of squared distances of samples to their closest cluster center.

### Fitting model to optimized K-value

### View the resulting graph
