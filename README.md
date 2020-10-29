# Vapour-Solvated Polymer Brushes
VSPB contains the LAMMPS input scripts for simulations of polymer brushes in equilibrium with solvent vapours.


## Usage
It contains two input files:

- `equi.in`, which takes a initial data file that can be generated using
[MDBrushGenerators](https://github.com/Compizfox/MDBrushGenerators) and which equilibrates the system by relaxing the
polymer brush. It outputs a `data.equi` file, which can be used further by `gcmc.in`.
- `gcmc.in` runs GCMC (Grand-Canonical Monte Carlo) to introduce solvent vapour particles into the system and outputs
  density profiles (among other things).

Both input files contain variables which values need to be specified using the LAMMPS `-var` CLI argument. The
`settings.ini` file is intended to be used with [Lampshade](https://github.com/Compizfox/Lampshade), which streamlines
the configuration-driven specification of these variable values for you.

## Publication
These input files are supplemental to the following paper:

Sorption Characteristics of Polymer Brushes in Equilibrium with Solvent Vapors  
Guido C. Ritsema van Eck, Lars B. Veldscholte, Jan H. W. H. Nijkamp, and Sissi de Beer  
Macromolecules 2020 53 (19), 8428-8437  
https://doi.org/10.1021/acs.macromol.0c01637  

## License
This repository is licensed under the GPL. See [LICENSE](LICENSE) for details.
