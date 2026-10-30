This repository contains the code accompanying the article:

# "Probabilistic Stellar Mass and Radius Estimation with Bayesian Hierarchical Stacking"
(https://arxiv.org/abs/2610.37968 [Accepted by A&A for publication])

The project implements a Bayesian machine learning framework for predicting stellar masses and radii of exoplanet host stars while fully propagating observational uncertainties and model variance.

## Abstract

### Context. 
Accurate stellar parameters are essential for the characterisation of exoplanets, yet most host stars lack direct measurements of mass and radius. These parameters set the inferred planetary properties, including radius, mass, and bulk density, with important implications for exoplanet physics, including potential habitability and the search for biomarkers.

### Aims. 
We aim to predict stellar masses and radii from commonly available observables and to quantify uncertainties and systematic effects in a way that is consistent with stellar observations. By not relying on a single Bayesian machine learning model, we aim to obtain more robust predictive distributions and reduce sensitivity to model misspecification and outliers.

### Methods. 
We develop a Bayesian machine-learning framework that combines three probabilistic models through Bayesian hierarchical stacking (BHS): a Bayesian additive regression tree model, a two-process heteroscedastic sparse Gaussian process, and a hierarchical Bayesian neural network. The method propagates measurement uncertainties, accounts for correlations among inputs, and aggregates model variance into final predictive distributions.

### Results. 
On a held-out test set the method attains a mean absolute relative difference (MARD) of 3.5% for mass and 2.1% for radius, improving on empirical-relation-based methods and standard machine-learning baselines. For 44 Kepler LEGACY stars, the BHS masses differ from estimates obtained with the BAyesian STellar Algorithm (BASTA) by a MARD of 4.8 per cent, compared with 8.5 per cent between the empirical relations and BASTA. Applied to about 2400 exoplanet host stars, the predictions differ from literature values by a MARD of 2.7% in both mass and radius. Residual analysis reveals mild underestimation for cool dwarfs, consistent with sparse training coverage, and positive offsets near the main-sequence turn-off that may reflect priors in isochrone-based catalogues. Internal consistency with g = GM/R2 is greater for the BHS predictions, with a scatter in ∆ log g lower by a factor of three than that of the literature values.
