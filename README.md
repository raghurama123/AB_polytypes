# AB Polytypes 

<a>
<center><img src="https://github.com/raghurama123/AB_polytypes/blob/main/4H.jpeg"  height="250"></center>
</a>

The purpose of this repository is to collect codes and data used in our paper ["Bandgaps of long-period polytypes of IV, IV-IV, and III-V semiconductors estimated with an Ising-type additivity model"](https://doi.org/10.1063/5.0166149).  

Feel free to write to me (ramakrishnan@tifrh.res.in) for further information.

# Codes
- [hk2AB.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/hk2AB.ipynb) converts `hk` sequences such as `hh, kkk, khkh` to the corresponding `AB` sequences `AB, ABC, ABAC`.
- [AB2haegg.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/AB2Haegg.ipynb) converts `AB` sequences such as `AB, ABC, ABAC` to the corresponding Haegg notation `+-, +++, +--+`.
- [MakeGeoms.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/MakeGeoms.ipynb) takes as inputs the stacking sequence (such as 'AB') and the elements ('Si' and 'C' for A and B) creates geometry.in for symmetry constrained geometry optimization using FHI-aims. 
- [DrawPolytypes.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/DrawPolytypes.ipynb) draws the structures of stacking arrangement of polytypes as viewed from the [10-10] plane of the hexagonal unit cell as shown in Fig. 1 of our paper. 
- [StoichiometricMatrix.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/StoichiometricMatrix.ipynb) creates the stoichiometric matrix used for ANNNI modeling. Each row corresponds to the terms in the Hamiltonian of a polytype. Columns correspond the the coefficient of J0, -J1, -J2, -J3, and -K of equation 4 of our paper. These coefficients (expect J0, which is 1 for all polytypes) are collected in Table II of our paper.
- [Fit_ANNNI.ipynb](https://github.com/raghurama123/AB_polytypes/blob/main/ipynb/Fit_ANNNI.ipynb) fits Model-4 to HSE03 band gaps and prints the model parameters listed in Table V of our paper.


# AB Polytypes dataset
FHI-aims input/output files 15 polytypes of 15 compositions are collected at [https://doi.org/10.17172/NOMAD/2024.01.18-1](https://doi.org/10.17172/NOMAD/2024.01.18-1)
- PBE lattice optimization
- PBE, SCAN, HSE06 electronic band structures
- For SiC, additionally, phonon band structures at the PBE level are provided for the long polytypes 9R, 12R, 15R1, and 15R2


# References
- _Bandgaps of long-period polytypes of IV, IV-IV, and III-V semiconductors estimated with an Ising-type additivity model_    
Raghunathan Ramakrishnan, Shruti Jain    
Journal of Chemical Physics, 159 (2023) 124702 (1-16).   
[https://doi.org/10.1063/5.0166149](https://doi.org/10.1063/5.0166149)      
See also the [Supplementary materials (zip file)](https://pubs.aip.org/jcp/article-supplement/2912689/zip/124702_1_5.0166149.suppl_material/)

```
@article{ramakrishnan2023bandgaps,
  title={Bandgaps of long-period polytypes of IV, IV-IV, and III-V semiconductors estimated with an Ising-type additivity model},
  author={Ramakrishnan, Raghunathan and Jain, Shruti},
  journal={The Journal of Chemical Physics},
  volume={159},
  number={12},
  year={2023},
  url={https://doi.org/10.1063/5.0166149},
  publisher={AIP Publishing}
}
```
