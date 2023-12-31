# Marginal and Paired Feature Screening for Ultrahigh-dimensional Binary Classification

Methods for screening marginal and paired features for two-class classification problems,
particularly well-suited for ultrahigh-dimensional data.

The methods are based on the concept of `energy distance` for the screening part, which also
leads to a natural coherence with "energy-based" classifiers. There are three separate algorithms:

    (a) MarS  - for screening marginal features
    (b) PairS - for screening paired features
    (c) MixS  - for screening marginal and paired features simultaneously

Instructions for using the codes are given below.

## Instructions:

There are three files that are necessary to execute the screening and classification
procedures proposed in the manuscript and its supplementary material:

1. The first file is an R-project titled ‘ExactScreening.Rproj’.
2. The other two files are R-scripts: a) SimulationStudy.R, and b)
relevant_functions.R.
3. The main script is SimulationStudy.R, which generates numerical results for 16
examples considered in the manuscript and supplementary material. This script calls
the user-defined functions necessary for executing different stages of screening and
classification, which are stored in relevant_functions.R. These functions include MV-
SIS, RRS, KF, and MCS-SVM, which screen variables using existing methods
(see the paper for details).
5. In addition to the existing screening methods, the proposed screening methods,
MarS and MixS, are also evaluated using different choices of the gamma function.
The results are stored in a .csv format file.

How to use:
1. Download and save the files to a single folder. 
2. Open the ExactScreening.Rproj file in RStudio.
3. Source the SimulationStudy.R script.
4. If RStudio is running on Windows, type "W" when prompted. Otherwise, type "O"
(see line 7 of SimulationStudy.R).
5. The numerical results for the 16 examples will be generated sequentially, starting
from example 1. The user can change the order in which the examples are executed,
and select which examples to run (see line 10 of the main script).

It is recommended to use the latest version of R for running the simulations.

## Reference: 

Roy, S., Sarkar, S., Dutta, S., and Ghosh, A. K. (2023) On Exact Feature Screening in Ultrahigh-dimensional Binary Classification
__[*arXiv preprint*](https://doi.org/10.48550/arXiv.2205.03831)__
