# Protein-Ligand Docking and MD Simulation Analysis

This repository contains the complete assignment regarding the molecular docking and molecular dynamics (MD) simulation for a specified protein-ligand complex (DQ2.5 / glia gama5). 

## Directory Structure

- **Docking Files/**: Contains the files related to the molecular docking process using Autodock Vina.
  - `Inputs/`: Structural files (PDB and PDBQT) for both the protein and the ligand.
  - `Outputs/`: Results of the docking process, including `.pdbqt` docked poses, the configured `.txt` grid box, and the Vina result log.
  - `Visualizations/`: Snapshots and figures illustrating the native interactions and the identified best-docked pose overlay.
  
- **Simulation Files/**: Covers the trajectories and configuration files for the 10 ns MD simulation using GROMACS.
  - `MD/`: Molecular dynamics pipeline outputs including topology (`.top`), binary run inputs (`.tpr`), coordinate (`.gro`), and trajectory (`.xtc`) files for energy minimization, NVT, NPT, and final production MD stages.
  - `Logs/`: Detailed `.log` files capturing the status of each simulation step.

- **`19_assignment2_Report.pdf`**: The comprehensive final report documenting the entire methodology, parameters utilized (like grid box sizing and GROMACS protocols), generated results, and analysis plots.

## How to use

1. The `.txt` files in `Docking Files/Outputs` can be reviewed for raw docking score metrics.
2. Structure visualizations can be viewed in PyMol or VMD using the corresponding `.pdb` and `.pdbqt` structures in combination with `.xtc` trajectory files. 
3. The report acts as the main reference for interpreting all simulation and docking outputs.
