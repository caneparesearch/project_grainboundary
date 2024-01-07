# Repository Description
This repository contains the data of the paper of W. Xie *et al.*, **Effects of Grain Boundaries and Surfaces on Electronic and Mechanical Properties of Solid Electrolytes** *Adv. Energy Mater.*,  (2023), DOI: [10.1002/aenm.202304230](https://doi.org/10.1002/aenm.202304230)

If our data and methodology contribute to your research, you're kindly asked to cited the manuscript mentioned above.
For additional information please e-mail us at the address found at [caneparesearch.org](https://caneparesearch.org)

# Introduction on the directory

## Folder: JSON_metadata

Folder **JSON_metadata** contains data extracted from the density functional theory (DFT) calculations, using the [Vienna Ab-initio Simulation Package](https://vasp.at) (VASP). Data is organized in subfolders, one per each material consider. Each folder contains a JSON file for each structure computed.

### File: miller_shift.json
The **miller_shift.json** is a JSON file containing the original data of the surface structure or the grain boundary structure.
For slab models, miller_shift.json contains the following quantities:
- final_energy: the calculated DFT total energy of this structure
- gamma: the surface energy in J m<sup>-2</sup>
- work_function: the work function of this slab model if calculated in eV
- ionization_potentail: the ionization potential of the slab model in eV, if calculated
- electron_affinity: the electron affinity of the slab model in eV, if calculated
- is_stochiometric: if the slab model is stochiometric or not
- incar_parameters: the VASP, INCAR file used to relax the slab model
- relaxed_structures: the relaxed structure in the format of a JSON dictionary. This file can be imported by [pymatgen](https://pymatgen.org) 
- formula: the chemical formula of this structure
- bandgap: bandgap in eV of this structure using GGA
- slab_thickness: thickness of this slab in &Aring;

For grain boundary models, the **miller_shift.json** file contains the following quantities:
- final_energy: the calculated DFT total energy of this structure
- sigma: the grain boundary excess energy in J m<sup>-2</sup>
- incar_parameters: the VASP, INCAR file used to relax used to relax the grain boundary model. 
- relaxed_structures: the relaxed structure in the format of a JSON dictionary. This file can be imported by [pymatgen](https://pymatgen.org)  
- formula: chemical formula of this structure
- bandgap: bandgap in eV of this structure using GGA


