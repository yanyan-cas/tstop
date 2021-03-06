#Time-series Topology (TS-TOP)
Release Date: June 2016

This project contains the source code and datasets for the time-series topology data analysis  tool suite for time-series characterization and classification as described in the  [paper](http://www.cv-foundation.org//openaccess/content_cvpr_2016_workshops/w23/papers/Seversky_On_Time-Series_Topological_CVPR_2016_paper.pdf) :

Seversky, Lee M., Shelby Davis, and Matthew Berger. 
"On Time-Series Topological Data Analysis: New Data and Opportunities." 
Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition Workshops. 2016.


If you use the software or associated data please use the following citation:

```
@InProceedings{Seversky_2016_CVPR_Workshops,
author = {Seversky, Lee M. and Davis, Shelby and Berger, Matthew},
title = {On Time-Series Topological Data Analysis: New Data and Opportunities},
booktitle = {The IEEE Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2016}
}
```

# Installation

## Exterior Sources to be downloaded:

From Arnur Nigmetov (Graz Unvirsity of Technology, Graz, Austria)

Download and Extract
[Hera] (https://bitbucket.org/grey_narn/hera/downloads)

Move `geom_bottleneck` to `tstop/ext/geom_dist/bottleneck` 

Move `geom_matching` to `tstop/ext/geom_dist/wasserstein` 


From David M. Mount and Sunil Arya (University of Maryland, College Park, Maryland)

Download [ANN](http://www.cs.umd.edu/~mount/ANN/) and extract to `tstop/ext/ANN`

## Building

Install [boost](http://www.boost.org) python and serialization libraries,
[scikit-learn](http://scikit-learn.org/stable/install.html),
[matplotlib](http://matplotlib.org/), 
[Eigen 3](http://eigen.tuxfamily.org/index.php),
[cmake](https://cmake.org/), and optionally [wxPython](https://wxpython.org/)
On machines with `apt-get`:
```sh
$ sudo apt-get install libboost-python-dev libboost-serialization-dev python-matplotlib python-sklearn python-wxgtk3.0-dev libeigen3-dev cmake
```


Run in `tstop`
```sh
$ cmake -DCMAKE_BUILD_TYPE=release .
$ make 
```

# Running

Add `tstop/python` to the `PYTHONPATH` environment variable 

# Documentation and Tutorial

For detailed documentation please see: [Documentation] (python/persistence/README.md)

For a short tutorial please see: [Time-series Topology Tutorial] (python/persistence/tutorial.md)


# Data

Time-series datasets and precomputed topological features: [Download] (https://drive.google.com/open?id=0B-eHoAvCU5B5M3dMS3VQWU5IRzA)

