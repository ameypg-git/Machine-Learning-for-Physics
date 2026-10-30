# Machine Learning for Physics

Coursework from **UCLA Physics C170M/270M, Machine Learning for Physics (Winter 2026)**:
six labs that work through the standard ML toolkit on physics and astronomy
datasets, and a final project on flow matching over curved data manifolds.
Lab partner and final-project co-author: Sven Harder.

<p align="center">
  <img src="assets/manifold_flows.png" width="760" alt="Source (blue) and target (red) distributions on a sphere, a torus and a genus-2 surface">
</p>

## Final project: Aspects of Flow Matching

Flow matching moves one data distribution into another along learned
trajectories. Ordinary flow matching draws straight lines in the ambient
space, which cut through the interior of a curved surface. We instead
learn a metric from the data (a K-Means/RBF construction), train one network
to produce geodesics of that metric as curved interpolants, and train a second
network to learn the velocity field along them. The method transports
data successfully on genus-0, genus-1 and genus-2 surfaces.

[Report (PDF)](Final%20Project/Aspects_of_Flow_Matching_report.pdf) ·
[Notebook](Final%20Project/flow_matching_on_manifolds.ipynb)

## Labs

| Lab | Topic | Methods | Files |
|:--|:--|:--|:--|
| [1](Lab%201) | Probability, Python and data exploration | NumPy broadcasting, pandas, exploratory plots of the Iris dataset | notebook, report |
| [2](Lab%202) | Classifying stars at the Galactic Center | Naive Bayes from scratch; feature engineering on stellar spectra (equivalent widths, cross-correlation) | notebook, data, report |
| [3](Lab%203) | Particle-physics event classification | Decision trees and random forests separating four-top from tt̄ events; handwritten digits | report |
| [4](Lab%204) | Neural networks | (a) a feed-forward network written from scratch in NumPy; (b) a Keras model of COVID-19 case data | reports |
| [5](Lab%205) | Unsupervised learning on stellar populations | K-Means, Gaussian mixtures and Bayesian GMMs in stellar velocity and chemical space | report |
| [6](Lab%206) | Mauna Loa CO₂ forecasting | Gaussian-process regression with composite kernels, chosen by log marginal likelihood | report |

**Tools:** Python · NumPy · pandas · scikit-learn · Keras/PyTorch · Matplotlib/Seaborn · Jupyter
