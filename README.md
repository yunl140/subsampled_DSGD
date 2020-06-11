# subsampled_DSGD
## Introduction
This repo implements the subsampled DSGD algortihm and tests the algorithm on two tasks, namely binary classification for the sklearn.make_moon dataset, and regression for the a residential energy consumption dataset (https://archive.ics.uci.edu/ml/datasets/Appliances+energy+prediction) 

## How to run the codes
The test case for classification can be run from terminal by 
```
python make_moon_classification.py
```
The test case for regression can be run from terminal by
```
python energy_regression.py
```
The supported input arguments are:
```
  -num_nodes          number of nodes in the network, default 10
  -samples_per_node   size of local dataset, default 1000
  -num_test_samples   number of samples in test set, default 2000
  -num_realizations   number of repeated experiments, default 1
  -max_iters          number of training iterations, default 1000
  -subsample_ratio    subsampling ratio in the subsampled DSGD algorithm, default 1.0 (no subsample)
  -gtype              type of network ('full' or 'ring'), default 'full'
  -ring_nbrs          number of neighbors on each side for the ring network, default 1
  -save_data          whether or not to save the simulated data, default False
```
