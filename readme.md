# Bayesian Regression With Undirected Network Predictors With an Application to Brain Connectome Data

# Author Contributions Checklist Form

## Data

### Abstract

Dataset provided: Simu1Case1Data.Rdata

Simulated Data for Case 1 – Simulation 1 (Xmat of dimension 70 X 190, y of length 70)

### Availability

The real data is available publicly at the following website:

http://m2g.io/

The processed real data as well as simulated datasets will be made
public eventually on the *github.com* page of the lead author.

### Description

*Permissions (demonstrate that author has legitimate access to data)*

The authors have taken permission from the original data providers. In
lieu, the data providers have requested to authors to cite their related
work and the authors have done the same.

*Licensing information*

The raw data as well as processed data as finally used will be uploaded
on the *github.com* webpage of the lead author.

*File format*

The original network graphs were in the "gpickle" format (which is a
NetworkX (Python library for graph analysis) format), and have been
converted to a graphml format readable by R.

The final converted data is available in .Rdata format.

*Metadata (including data dictionary)*

The final data used by the authors consist of a predictor matrix Xmat
(dimension 79 X 2278 for real application, dimension 70 X 190 for
simulated scenario) and continuous response vector y (length 79 for real
application, length 70 for simulated scenario).

## Code


### Abstract

1.  BNSPCodeRun.R- The code loads the data in .Rdata format (‘Xmat’ is
    the predictor and ‘y’ is the continuous response). It then sources
    the code BNSP-Function.R, which consists of a function to input data
    and parameters to run the BNSP model. Subsequently, the MCMC chain
    (using Gibbs sampler) is run for niter = 50000 iterations. Model
    performance in terms of mean squared error of edge detection and
    also probability of node detection is then calculated.

2.  BNSP-Function.R – The code contains function ‘BNSPfunc’ that inputs
    data and relevant parameters to run the BNSP model.

### Description

The R code will be delivered as a .R file.

R libraries used are listed in the R code supplied.

## Instructions for Use

### Reproducibility

BNSPCodeRun.R can be used to reproduce Figures 2 and 3; Tables 4, 5 and 6 (Node selection probabilities) by changing the simulation settings. We have provided simulated data for Simulation 1 (Case 1).

