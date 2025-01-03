# Gaussian-Mixture-Model

# Overview

This assignment focuses on clustering analysis using the data provided in the HW11-ClusteringData.csv file. The dataset contains 1600 2D data points generated using a Gaussian mixture model with four components. The goal is to perform clustering using various techniques, evaluate the results, and compare the estimated parameters with the true parameters.

# Tasks

<ins> Data Visualization</ins>

**Objective**: Plot the data points using different colors based on their labels.

**Details**:

Each row in the dataset corresponds to a single data point.

The first two columns contain the coordinates of the data points.

The third column provides the true labels for reference.

<ins> K-Means Clustering</ins>

**Objective**: Cluster the data points using the k-means clustering algorithm for 𝑘 ∈ {2,3,4,5,6,7}.

**Evaluation**:

Use the silhouette score to evaluate the quality of clustering for each value of 𝑘.

The silhouette coefficient s(i) is defined as:

s(i) = (&#946;(i) - &#945;(i)) / max( &#945;(i), &#946;(i) )

where,

&#945;(i) = average distance to the other points in the same cluster.

&#946;(i) = minimum average distance to points in the nearest cluster.

**Implementation**:

Compute and plot the average silhouette score for each 𝑘 using:
   1. Euclidean distance
   2. Manhattan distance
Determine the optimal 𝑘 based on the maximum average silhouette score.

<ins> Expectation-Maximization (EM) Algorithm</ins>

**Objective**: Use the EM algorithm to estimate:

  1. Mixture probabilities &#960;<sub>k</sub>.

  2. Mean vectors &#956;<sub>k</sub>, where k ∈ {1,2,3,4}.

**Comparison**:

Compare the estimated &#960;<sub>k</sub> and &#956;<sub>k</sub> values with the true values:

   μ1=[4,6], μ2=[−3,3], μ3=[2,−2], μ4=[−1,−7]
  
   &#960; = (0.1875,0.25,0.3438,0.2188)

**Visualization**:

Plot the Gaussian mixture model distribution using the estimated parameters.

Options:

  Probability density function

  Contour Plot


  # Tools and Libraries

  Python

  NumPy

  Pandas

  Matplotlib

  Seaborn

  sklearn
