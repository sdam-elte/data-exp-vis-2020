### 1. File formats
Historically many softwares that produced a large amount of output created its own file format. Softwares doing classical molecular dynamics, density functional theory calculations, Quantum Monte Carlo etc not only produce data for the user as an end result, but also generates data that are reused during iterative calculations or saved as checkpoints in case of failure. These data are/were stored in custom defined binary files first and later with the spread of standardised file formats such as cube, hdf5, netcdf etc. data became much easy to transfer.

#### Hierarchical Data Format (**HDF5**) -
Useful links:
* https://www.hdfgroup.org/solutions/hdf5/
* Numpy npz versus hdf5: https://stackoverflow.com/questions/27710245/is-there-an-analysis-speed-or-memory-usage-advantage-to-using-hdf5-for-large-arr
* Why not to use hdf5: https://cyrille.rossant.net/moving-away-hdf5/
* About B-trees: https://www.youtube.com/watch?v=aZjYr87r1b8

#### The Network Common Data Form (**netcdf**) 
https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_introduction.html

