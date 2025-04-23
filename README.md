# MAPD_ModB_Project
Authors: Laura Marie Schulze, Maria Camila Paris Diaz, Lorenzo Martinelli

Project for the second half of the course Management and Analysis of Physics Datasets, part of the master's degree cycle in Physics of Data delivered at UNIPD

## Outline
The goal of this project is to produce a pipeline that effectively reconstructs the trajectories described by cosmic rays crossing through drift chambers in at the INFN center in Legnaro (PD). The project's other goal, however, is to develop such a pipeline fully leveraging on parallel processing capabilities. This result is achieved by employing three virtual machines working as a cluster. The framework of choice for this project was chosen to be Dask, as it allowed to easily outscale the data analysis pipeline with minimal changes in the way the syntax is laid out. 

On a more "scientific" note, the project deals with reconstructing trajectories on a first approximation, hence a simple least squares fit has been employed. Additionally, some techniques have been explored to deal with outliers, with the underlying idea being taking advantage of the geometry of the chambers. On a more "informatic" note, the second file, called `MAPD_Gr10_Benchmarking.ipynb`, was used to assess the time taken to carry out the process spanning through a great amount of possible configurations in the cluster. 

The whole project has been carried out in Python.
