# pyKrack

<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

![CI](https://github.com/FerranC96/pyKrack/actions/workflows/test.yaml/badge.svg)
[![PyPI
version](https://badge.fury.io/py/pykrack.svg)](https://badge.fury.io/py/pykrack)

## Install

Due to the comparisons with the R package `sna` we recommend using conda
to manage your environment.

1.  First create the pykrack conda environment from the environment.yml
    file:

``` sh
conda (or mamba) env create -f environment.yml
```

2.  Then load the conda environment with:

``` sh
conda activate pykrack
```

3.  And finally install the package from pip via the following command:

``` sh
pip install pyKrack
```

Alternatively pyKrack can also be isntalled using pip via the following
command

``` sh
pip install pyKrack
```

Then install the R dependencies listed in the conda environmnet.yml
manually.

## How to use

Please see the core and hierarchy notebooks for more detailed
explanations.

**pyKrack** consists of one main function,
[`compute_hierarchy`](https://FerranC96.github.io/pykrack/hierarchy.html#compute_hierarchy).

------------------------------------------------------------------------

<a
href="https://github.com/FerranC96/pykrack/blob/main/pykrack/hierarchy.py#LNone"
target="_blank" style="float:right; font-size:smaller">source</a>

### compute_hierarchy

>      compute_hierarchy (G, metric='pykrack')

Compute one of the possible hierarchy scores

|             | **Type**  | **Default** | **Details**                                                                                                                                                                                                                                                            |
|-------------|-----------|-------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| G           |           |             | Directed NetworkX graph                                                                                                                                                                                                                                                |
| metric      | str       | pykrack     | Type of hierarchy metric to compute. Accepted types are:<br>‘pykrack’ for this module’s implementation of the Krackhardt score.<br>‘rsnakrack’ for the sna implementation in R.<br>‘hierarchy_flow’ for the Luo and Magee 2011 as implemented in the NetworkX package. |
| **Returns** | **float** |             | **One of the possible hierarchy scores**                                                                                                                                                                                                                               |
