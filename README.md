# Repository Descrption
This repository contains the data of the paper *add link*
If our data fortunately contribute to your research, please consider cite us at *add doi*

# Introduction on the directory

## JSON_metadata

is the folder containing the data involved of DFT calculation using Vienna Ab-initio Simulation Package (VASP). The subfolder are the materials, and contianing json file of each calculated structures.

### miller_shift.json
This is the json file containing the original data for the  surface or grain boundary.
For slab model it contains
- final_energy: calculated total energy of this structure
- gamma: surface energy in Jouls per meter squared
- work_function: work function of this slab model if calculated
- ionization_potentail: ionization potential of this slab model if calculated
- electron_affinity: electron affinity of this slab model if calculated
- is_stochiometric: whether the slab model is stochiometric or not
- incar_parameters: the INCAR paramter used to relax the slab model
- relaxed_structures: the relaxed structure in the format of dictionary, and can be read by pymatgen
- formula: chemical formula of this structure
- bandgap: bandgap of this structure using GGA
- slab_thickness: thickness of this slab in Angstrom

For grain boundary, it contains:
- final_energy: calculated total energy of this structure
- sigma: grain boundary excess energy in Jouls per meter squared
- incar_parameters: the INCAR paramter used to relax the slab model
- relaxed_structures: the relaxed structure in the format of dictionary, and can be read by pymatgen
- formula: chemical formula of this structure
- bandgap: bandgap of this structure using GGA

