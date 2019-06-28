# SubCluGen
A simple datagenerator in Python for generating data sets with subspace clusters

# Updates:
Version 1.0:
  * TBA
  
Version 0.3:
  * Needs fix for a specific combination of cluster shapes, now overrides some cluster numbers 
  * First Upload 

# Instructions: 
How to use:

The function generate_subspacedata([args]) needs the following parameters:

* n (int): The number of points you want to have in your dataset

* d (int): The number of dimensions per point

* mu_clu (bool): Can one point be included in multiple subspaces? [Default:False]

* [Optional] subspaces (ndarray): A list of subspaces you want to have in your dataset, written in the following way:

[[sub_n, sub_d, c, std], ... ] with

* sub_n   (int): number of points in this subspace

* sub_d   (int): number of dimensions in this subspace

* c (int): number of clusters in this subspace

*   std (float): the standard derivation of the cluster(s)

# Example:
A, lables = generate_subspacedata(10, 10, True, [[2, 4, 1, 1.0], [3, 2, 2, 1.0], [6, 3, 1, 0.4], [4, 9, 1, 0.6]])
