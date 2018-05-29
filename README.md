# Riemannian Procrustes Analysis

This repository contains Python code for using the Riemannian Procrustes Analysis method proposed in [1]. This procedure is a Transfer Learning approach for dealing with the statistical variability of EEG signals recorded on different sessions and/or from different subjects. This is a common problem faced by Brain-Computer Interfaces (BCI) and poses a challenge for systems that try to reuse data from previous recordings to avoid a calibration phase for new users. 

RPA is based on the concept of Procrustes analysis [2]. It works by matching the statistical distributions of two datasets using simple geometrical transformations (translation, scaling and rotation) over the data points in both datasets. We use symmetric positive definite matrices (SPD) as statistical features for describing the EEG signals, so the geometrical operations on the data points respect the intrinsic geometry of the SPD manifold. 

We have included two notebooks with examples of application of the RPA on data from two BCI paradigms : motor imagery and SSVEP. Both notebooks are self-explanatory and illustrate the improvement in cross-subject classification when RPA is used as a step for matching the statistical distributions of the datasets.

[1] Pedro L. C. Rodrigues, Christian Jutten, and Marco Congedo - "*Riemannian Procrustes Analysis : Transfer Learning for Brain-Computer Interfaces*", submitted to IEEE Transactions on Biomedical Engineering in May 2018. Please send an e-mail to `pedro.rodrigues@gipsa-lab.fr` if you want a copy of the manuscript.

[2] J. C. Gower and G. B. Dijksterhuis, "*Procrustes Problems*". Oxford University Press, January 2004
