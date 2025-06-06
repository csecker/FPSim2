[![CI Testing](https://github.com/chembl/FPSim2/workflows/CI/badge.svg)](https://github.com/chembl/FPSim2/actions?query=workflow%3ACI+branch%3Amaster)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/fpsim2.svg)](https://anaconda.org/conda-forge/fpsim2)
[![Downloads](https://pepy.tech/badge/fpsim2)](https://pepy.tech/project/fpsim2)
[![DOI](https://zenodo.org/badge/154705090.svg)](https://zenodo.org/badge/latestdoi/154705090)


# FPSim2: Simple package for fast molecular similarity searches

FPSim2 is a small NumPy centric Python/C++ RDKit based package to run fast compound similarity searches. FPSim2 performs better with high search thresholds (>=0.7). Currently used in the [ChEMBL](http://www.ebi.ac.uk/chembl/) and [SureChEMBL](https://www.surechembl.org/) interfaces.

Highlights:
- Uses CPU POPCNT instruction for fast bit counting
- Bounds for sublinear speedups from [10.1021/ci600358f](https://pubs.acs.org/doi/abs/10.1021/ci600358f)
- A compressed file format with optimised read speed based in [PyTables](https://www.pytables.org/) and [BLOSC2](http://www.blosc.org/pages/blosc-in-depth/)
- Fast multicore CPU and GPU similarity searches
- In memory and on disk search modes
- Distance matrix calculation

## Installation

With [pip](https://pypi.org/project/FPSim2/):

```bash
pip install fpsim2
```

With [conda](https://anaconda.org/conda-forge/fpsim2):

```bash
conda install conda-forge::fpsim2
```

With [SBGrid](https://sbgrid.org/software/titles/fpsim2):
```
sbgrid-cli install fpsim2
```

## Documentation

Documentation is available at https://chembl.github.io/FPSim2/


## Trying it online

To try out FPSim2 interactively in your web browser, check out this Google Colab notebook [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1E-Hu0YXHb4aaVQWOLzMTJFdAhh3nIbxA)
