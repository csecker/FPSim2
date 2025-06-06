# FPSim2's documentation

[FPSim2](https://github.com/chembl/FPSim2) is a NumPy-centric Python/C++ package for running fast compound similarity searches. FPSim2 performs optimally with high search thresholds (>=0.7). It is currently used in the [ChEMBL](https://www.ebi.ac.uk/chembl/) and [SureChEMBL](https://www.surechembl.org) interfaces.

## Highlights

- Uses CPU POPCNT instruction for fast bit counting
- Implements bounds for sublinear speedups from [10.1021/ci600358f](https://pubs.acs.org/doi/abs/10.1021/ci600358f/)
- Features a compressed file format with optimized read speed based on [PyTables](https://www.pytables.org/) and [BLOSC2](http://www.blosc.org/pages/blosc-in-depth/)
- Provides fast multicore CPU and GPU similarity searches
- Supports in-memory and on-disk search modes
- Enables distance matrix calculation

## Getting started

Install and generate a FPSim2 fingerprint db file.

- [Installation](user_guide/install.md)
- [Create a fingerprint db file](user_guide/create_db_file.md)
- [Sanitization](user_guide/sanitization.md)
- [Alternative SQLAlchemy backend](user_guide/sql_backend.md)


## CPU searches

Learn how to run CPU based similarity searches:

- [Run symmetric similarity searches](user_guide/similarity.md)
- [Run Tversky asymmetric searches](user_guide/tversky.md)
- [Run substructure screenouts](user_guide/subs_screenout.md)
- [Generate a symmetric distance matrix](user_guide/sim_matrix.md)

## GPU searches

Learn how to run GPU based similarity searches:

- [Run GPU based Tanimoto similarity searches](user_guide/gpu.md)
