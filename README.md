# WISC Windstorm Loss and Risk Model

Python implementation of the WISC (Windstorm Information Service) Loss and Risk model.

Please refer to the [ReadTheDocs](http://wisc.readthedocs.io/) of this project for the full documentation of all functions. 

**Requirements:** [NumPy](http://www.numpy.org/), [pandas](https://pandas.pydata.org/), [geopandas](http://geopandas.org/), [seaborn](https://seaborn.pydata.org/), [matplotlib](https://matplotlib.org/)

**Core Report:** [Koks et al., 2017](https://wisc.climate.copernicus.eu/wisc/documents/shared/C3S_WISC_Tier%203_Indicator_Descriptions_v1.0.pdf)

```
Koks, E.E., Tiggeloven, T., Coumou D., Aerts, J.C.J.H., Whitelaw A. (2017) 
WISC Risk and Loss Indicator Descriptions. Copernicus Climate Change Service.
```

**Sensitivity Analysis:** [Koks et al., 2017](https://wisc.climate.copernicus.eu/wisc/documents/shared/(C3S_441_Lot3_WISC_SC2-D5.2-VU-RP-17-0084)%20(Case%20Study%20-%20Tier%203%20Indicators%20Sensitivity%20Analysis)%20(1.0).pdf)

```
Koks, E.E., Coumou D., Aerts, J.C.J.H.,(2017) 
WISC Case Study: Tier 3 Indicators Sensitivity Analysis. Copernicus Climate Change Service.
```

## Prepare data paths

Copy `config.template.json` to `config.json` and edit the paths for data and
figures, for example:

```json
{
    "data_path": "/home/<user>/projects/WISC/data",
    "figures_path": "/home/<user>/projects/WISC/figures"
}
```

## Python requirements

Recommended option is to use a [miniconda](https://conda.io/miniconda.html)
environment to work in for this project, relying on conda to handle some of the
trickier library dependencies.

```bash

# Add conda-forge channel for extra packages
conda config --add channels conda-forge

# Create a conda environment for the project and install packages
conda env create -f environment.yml
activate WISC

```


### License
Copyright (C) 2018 Elco Koks. All versions released under the [MIT license](LICENSE.md).