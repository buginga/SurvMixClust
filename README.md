# SurvMixClust

This repository contains the code for the model present in the paper X. It structures its use using the functions fit, predict and training similar to scikit-learn API.

```latex

```
 
## Model

SurvMix Clust is a finite mixture of nonparametric distributions, using the features to model the mixture proportions with a multinomial logistic regression. In other words, it's a mixture of experts with a gating network for the right-censored time-to-event clusterization problem. It's trained via maximum likelihood with a variety of the Expectation-Maximization (EM) algorithm. Experimental evidence presented shows that our proposal generates competitive predictive performance, sharply different and informative clusters, and interpretable results.

![Model](figures/bayesian_net.png)


![Risk](figures/figure_comparing_clusterizations.png)


## Prerequisites
The code is implemented with the following dependencies:
- The R package [survPresmooth](https://cran.r-project.org/web/packages/survPresmooth/index.html) needs to installed. Then, rpy2 package is used to communicate with this package from inside python.

- still to be done, requirements.txt doesn't have the required packages. And needs to be tested if a pip install -r requirements.txt will going to work.  

```
pip install -r requirements.txt
```

## Data
We consider the following datasets:

- [SUPPORT](http://biostat.mc.vanderbilt.edu/wiki/Main/DataSets)
- [Flchain](https://vincentarelbundock.github.io/Rdatasets/doc/survival/flchain.html)
- METABRIC
- GBSG
- WHAS500

## Model Training

Please check the model_use.ipynb for a example of training and model use.


## Acknowledgments
