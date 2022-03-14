# Running Classifiers On Large Multiscale Temporal and Spectral Features
by Team 13 

## Getting Started

First, download the source code.
Then, download the dataset "Four class motor imagery (001-2014)" of the [BCI competition IV-2a](http://bnci-horizon-2020.eu/database/data-sets). Put all files of the dataset (A01T.mat-A09E.mat) into a subfolder within the project called 'dataset'. 

### Prerequisites

- python3
- numpy
- sklearn
- pyriemann
- scipy

The packages can be installed easily with conda and the _config.yml file: 
```
$ conda env create -f _config.yml -n msenv
$ source activate msenv 
```

### Recreate results

This code builds off of https://github.com/MultiScale-BCI/IV-2a. 

For the recreation of the CSP results run main_csp_compilation.py. 

```
$ python3 main_csp_compilation.py
```
For the recreation of the Riemannian results run main_riemannian_compilation.py.

```
$ python3 main_riemannian_compilation.py
```

