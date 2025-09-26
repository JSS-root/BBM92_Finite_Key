# BBM92 Finite Key


## Overview and description

Code base for the BBM92 finite key analysis protocol. This project numerically implements a finite-key solver for the BBM92 protocols.

Maximisation is performed using both direct optimisation and brute force approaches to enable user suitable tradeoffs in runtime.


## Author: Jasminder S Sidhu

## Directory Structure

```
BBM92_Finite_Key/
├── README.md                                   # Documentation
├── LICENSE                                     # MIT License
└── Solvers/
    ├── BBM92_BruteForce                        # optimiser using Brute force
    ├── BBM92_Opt                               # optimiser using direct optimisation
    ├── BBM92_BruteForce_Parallelised_SatQKD    # optimiser using direct optimisation, applied to SatQKD
```


## New features

The BBM92_Bruteforce_Parallelised_SatQKD file features the following updates:
    1. Parallelised version for optimisation parameters. Implements ThreadMapping. Block optimisation left sequential. 
    2. Key rate optimiser applied to SatQKD. Example loss file (clickfile_OGSsep_500km_phi_0_xi_0.csv) provided.
    3. Block optimisation implemented for a satellite overpass to maximise keys.
    4. Utilities: Input/output directories, runtime information, and line comments provided for easier edits. 

Modularity: Code is now modular:
    1. Module 1: Loss selection and profile
    2. Module 2: Block and error rate calculations
    3. Module 3: Finite key rate optimisation

    
## To-dos

Work is underway to translate code to Python.


## Citation and attribution

If you use this software in your research please cite as follows:


<pre>  
```
@software{Side_BBM92_2025,
author = {Sidhu, Jasminder Singh},
title = {{BBM92: Optimised finite key analyser for satellite links}},
url = {https://github.com/JSS-root/BBM92_Finite_Key/tree/main},
year = {2025}
}
```
</pre>

Associated documentation and application paper under development. 
