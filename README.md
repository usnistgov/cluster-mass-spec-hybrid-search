# cluster-mass-spec-hybrid-search

Implementation of techniques described in the manuscript 

**Clustering and Multidimensional Scaling of Hybrid Similarity Search Results: Application to Illicit Drug Mass Spectra**

Melinda A. Kleczynski (National Institute of Standards and Technology, Georgetown University)

Arun S. Moorthy (Trent University)

Anthony J. Kearsley (National Institute of Standards and Technology) anthony.kearsley@nist.gov

## Programming language and packages

* [Python](https://www.python.org/) 
* [Matplotlib](https://matplotlib.org/stable/) 
* [NumPy](https://numpy.org/doc/stable/index.html) 
* [pandas](https://pandas.pydata.org/) 
* [scikit-learn](https://scikit-learn.org/stable/index.html) 
* [SciPy](https://docs.scipy.org/doc/scipy/index.html) 

Certain equipment, instruments, software, or materials are identified in this paper in order to specify the experimental procedure adequately.
Such identification is not intended to imply recommendation or endorsement of any product or service by NIST, nor is it intended to imply 
that the materials or equipment identified are necessarily the best available for the purpose.

## Repository contents 

The "hitlists" folder contains the data (Names, NIST Numbers, Match Factors).

The "TwoStepClusterLabels" and "MdsClusterLabels" folders contain the cluster labels from the original HSS dissimilarities and the MDS configurations. 

The notebooks can be run in this order.
Plot formatting is slightly different than in the manuscript, due to space constraints in the manuscript but not the notebooks.

1. The "installs" notebook contains package installation instructions.

2. The "TwoStepClustering" notebook runs the two-step clustering procedure for the original HSS dissimilarities. This notebook produces the plots in Figures 2, 3, and 4.

3. The "MDS" notebook produces the multidimensional scaling (MDS) configurations. This notebook produces the plots in Figures 9, 10, 11, and 12. This notebook has the longest run time. The outputs are saved in the "configurations" folder, allowing the "CompareClustering" notebook to be run.

4. The "CompareClustering" notebook compares the cluster labels obtained from the original HSS dissimilarities to the cluster labels obtained from the MDS configurations and plots the MDS configurations with cluster labels. This notebook produces the plots in Figures 5, 6, 7, and 8. 
