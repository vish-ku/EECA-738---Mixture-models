# Overview

In this project I try to model data by using Mixture model methods (Gaussian distribution) using the expectation maximization algorithm. Two data sets were chose from UCI machine learning data repositories and we tried to classify the data set into sepecified number of cluster. The Expectation maximization method is an example of a soft 
clustering, in the sense that we get the probability of the data point belonging to a cluster rather than assigning it to the cluseter like in K-means algorithm. 

# Algorithm

In this model we choose randomly chosen gaussian functions and calculate the probability that the given data points are from the given gaussian. Then we calculate the posterior probability ( responsibilities )  of gaussians given the data points by applying bayes rule - This is the Expectation step. Once we have those we update the gaussian, i.e. that is we find the new means and covariance - this step is called the maximization step. The formula for the new means is derived by maximizing the log likelihood function of the gaussian mixture model. 

# Data sets

One of the data sets that I chose was the iris data set. This data has information collected form flowers regarding their Sepal and Petal width and length and we try to cluster the flowers based on these datas. 

The other data set that I selected was the Indian Liver Patient data set. The goal was to use the data parameters and cluster the data points to identify patients with liver disease. The algorithm could have been run with all of the data parameters, but for the sake of visualization I selected two data parameters, the total Bilirubin and the Albumin levels. 
