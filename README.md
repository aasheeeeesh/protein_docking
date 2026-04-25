<div align="center">
  
# 🧬 Protein-Ligand Docking & MD Simulation
**Exploring the DQ2.5 / glia gama5 complex at the nanoscale**

[![GROMACS](https://img.shields.io/badge/GROMACS-FF8000?style=for-the-badge&logo=linux&logoColor=white)]()
[![AutoDock Vina](https://img.shields.io/badge/AutoDock_Vina-0052CC?style=for-the-badge&logo=atom&logoColor=white)]()
[![PyMOL](https://img.shields.io/badge/PyMOL-20232A?style=for-the-badge&logo=python&logoColor=white)]()

⚙️ *A complete end-to-end structural bioinformatics pipeline featuring molecular docking and a blazing-fast 10 ns MD simulation.*
</div>

---

## 🔬 About the Project
This repository hosts the computational methodology, raw configuration data, and analysis plots for performing molecular docking and molecular dynamics (MD) on the selected biomolecular target. Whether you are delving into spatial grid configurations or analyzing trajectory fluctuations, everything is here.

<p align="center">
  <img src="Docking%20Files/Visualizations/docked_best_pose.png" width="45%" alt="Docked Pose" />
  <img src="Docking%20Files/Visualizations/overlay_screenshot.png" width="45%" alt="Overlay Validation" />
</p>
<p align="center"><i>Visualizing the optimal binding pocket interactions.</i></p>

## 📂 Repository Architecture

### 🧩 1. Docking Files (`/Docking Files`)
We utilized **AutoDock Vina** to compute optimal binding poses and scoring affinities. 
*   📁 **`Inputs/`**: Pristine PDB and PDBQT configurations for the protein-ligand duo.
*   📁 **`Outputs/`**: Docking hits! Includes grid box parameter mappings `.txt` and the final pose scores in `.pdbqt` and `.txt` log formats.
*   🖼️ **`Visualizations/`**: Graphical snapshots illustrating structural overlaps and grid alignments.

### 🌪️ 2. Simulation Files (`/Simulation Files`)
The complex was subjected to a 10 ns **GROMACS** molecular dynamics run to interrogate stability over time.
*   📁 **`MD/`**: The core run files. Contains topologies (`.top`), run inputs (`.tpr`), coordinates (`.gro`), and trajectory data (`.xtc`) spanning Energy Minimization, NVT/NPT Equilibration, and Production phases.
*   📑 **`Logs/`**: Comprehensive simulation log files detailing the progress of each step.
*   📈 **`Plots/`**: Rendered analysis plots measuring physical stability, including:
    *   *Root Mean Square Fluctuation (RMSF)*
    *   *Solvent Accessible Surface Area (SASA)*
    *   *Density, Temperature, Potential, and Pressure graphs*

### 📄 3. The Research Report
*   📚 **`19_assignment2_Report.pdf`**: The crown jewel—a meticulously documented report detailing the software tooling, protocol steps, methodology, and comprehensive interpretations of both docking affinities and MD trajectory stability.

---

## 🛠️ How to Dive In

1. **Read the Report:** Start with `19_assignment2_Report.pdf` to gain the full context of the experiment and results.
2. **Visualize the Data:** Open up the coordinate `.gro` and trajectory `.xtc` files in viewers like **PyMOL**, **VMD**, or **ChimeraX** for an interactive look at the atomic motion.
3. **Parse the Logs:** Check out the `.txt` outputs in `Docking Files/Outputs/` for raw numerical scoring metrics, or the `.log` files in `Simulation Files/Logs/` for thermodynamic verification.

> *"To understand the function of a biomolecule, one must first grasp its structure."* 🤖
