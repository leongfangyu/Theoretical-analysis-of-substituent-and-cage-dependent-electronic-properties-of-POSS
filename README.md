<div align="center">   
  
# Theoretical Analysis of Substituent- and Cage-dependent Electronic Properties of POSS
</div>

## [Paper](https://doi.org/10.1063/5.0150173)

## Abstract
Polyhedral Oligomeric Silsesquioxanes (POSS) molecules have emerged as promising alternatives to traditional silica nanoparticles and organosilicon molecules due to their ability to attach a variety of substituents to their central siloxane cages. The electronic features of POSS are dependent on the structures of substituents and cages, making them attractive for applications, such as drug nanocarriers, chemosensors, Janus particles, and inorganic–organic nanocomposites. However, the lack of detailed geometric data poses a difficulty in extending POSS studies using the force field method or beyond the quantum mechanical level. To lay a foundation for future experimental and computational studies, we present new theoretical insights into the influence of substituent and cage on the cage geometries (Si–O bond length, pore width, cage volume, etc.) of 16 substituted POSS molecules with various substituents and cages (T<sub>7</sub>, T<sub>8</sub>, T<sub>10</sub>, T<sub>12</sub>). Our results show that the mean Si–O bond length of the POSS cage can be in the range of 1.619–1.670 Å, depending on the substituent and cage. Moreover, we show that the expansion or shrinkage of POSS depends on the types of substituents, rather than the inductive effect of substituents. Our results demonstrate that the conformational stability, dipole moment, and polarizability of POSS depend on the substituents’ size, substituents’ shape, type of functional moieties of substituents, and cage size. In addition, the HOMO-LUMO bandgap of POSS can be tuned by changing the hydrocarbon chain length, number of aromatic rings, and types of functional groups on the substituents. Finally, we report several sets of geometric data that are transferable to the existing parametrization methods of force field models.

## Repository content and data availability

This repository provides **geometrically optimized structures of substituted
Polyhedral Oligomeric Silsesquioxanes (POSS)** obtained at the
**B3LYP/6-31+G(d)** level of theory. The optimized structures correspond to the POSS molecules investigated in the
associated publication and include variations in both **cage size**
(T<sub>7</sub>, T<sub>8</sub>, T<sub>10</sub>, T<sub>12</sub>) and
**substituent type**.

All structures are provided in **PDB format**, which can be readily converted
or reconstructed for use in:

- molecular dynamics simulations (e.g. **LAMMPS**),
- force-field-based modeling (e.g. **BIOVIA Materials Studio**),
- further **quantum-chemical calculations**, or
- geometry analysis and visualization workflows.

The availability of these optimized geometries is intended to **facilitate reuse and extension of POSS studies beyond the quantum-mechanical level**, in particular for force-field parametrization, adsorption modeling, and structure–property relationship analysis.



## Computational workflow

The geometries provided in this repository were generated using **Gaussian 16**.  
Geometry optimization and vibrational frequency verification were performed using the following procedure:

### Geometry optimization
The molecular structures were first optimized using:

#p opt b3lyp/6-31+g(d) em=gd3bj geom=connectivity


### Frequency calculation
After successful convergence of the optimized structure, vibrational frequency calculations were performed using:

#p freq b3lyp/6-31+g(d) em=gd3bj geom=connectivity


The frequency calculations were used to confirm that the optimized geometries correspond to local minima (no imaginary frequencies).

### Structure conversion and simulation preparation
The converged structures were subsequently exported into **PDB format** using **GaussView 6**. The PDB structures can be further imported into molecular system construction tools such as:

- **Packmol**
- **Moltemplate**

The generated molecular systems can then be used in simulation environments, including:

- **BIOVIA Materials Studio**
- **LAMMPS**


## Relation to published studies

The electronic and structural properties of the provided POSS geometries,
including:

- cage dimensions (Si–O bond length, pore width, cage volume),
- conformational stability,
- dipole moment and polarizability, and
- HOMO–LUMO bandgap trends,

are discussed and analyzed in the associated publication:

**Theoretical analysis of substituent- and cage-dependent electronic
properties of POSS**  
https://doi.org/10.1063/5.0150173

## Intended use

This repository is designed as an **open structural reference dataset** for
researchers working on:

- POSS-based nanomaterials,
- inorganic–organic hybrid systems,
- force-field development and validation,
- adsorption and encapsulation modeling, and
- structure–property analysis of functionalized silsesquioxanes.

Users are free to employ the provided geometries for further simulations and
analysis, with appropriate citation of the associated publication.


### BibTex
If this work is helpful for your research, please consider citing the following BibTeX entry.

```
@article{leong2023theoretical,
  title={Theoretical analysis of substituent-and cage-dependent electronic properties of POSS},
  author={Leong, Fang Yu and Low, Liang Ee and Chew, Irene Mei Leng},
  journal={AIP Advances},
  volume={13},
  number={6},
  year={2023},
  publisher={AIP Publishing},
}
