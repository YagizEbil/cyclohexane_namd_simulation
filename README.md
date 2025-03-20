# Conformational Map of Cyclohexane

## Project Overview

This repository contains files and scripts for running molecular dynamics simulations of cyclohexane using NAMD. The project involves setting up the simulation environment, running simulations at different temperatures, and analyzing the results to study the behavior of cyclohexane molecules.

## Features

- **Simulation Setup**: Includes `.pdb`, `.psf`, and `.prm` files for defining the molecular structure and parameters of cyclohexane.
- **Temperature Variations**: Simulations are run at multiple temperatures (e.g., 100K, 1000K, 1500K) to observe temperature-dependent behavior.
- **Trajectory Files**: `.dcd` files store the simulation trajectories for analysis.
- **Visualization**: Includes scripts and figures for visualizing density and potential of mean force (PMF) in 3D.
- **Analysis**: Provides tools for analyzing simulation results and generating reports.

## Repository Structure

```
cyclohexane_namd_simulation/
├── 1000k_run.dcd          # Trajectory file for 1000K simulation
├── 1000k_run.txt          # Log file for 1000K simulation
├── 100k_run.dcd           # Trajectory file for 100K simulation
├── 100k_run.txt           # Log file for 100K simulation
├── 1500k_run.dcd          # Trajectory file for 1500K simulation
├── 1500k_run.txt          # Log file for 1500K simulation
├── cyclohexane.namd       # NAMD configuration file
├── cyclohexane.pdb        # Cyclohexane molecular structure file
├── cyclohexane.psf        # Cyclohexane protein structure file
├── main.ipynb             # Jupyter notebook for analysis and visualization
├── par_all35_ethers.prm   # Parameter file for ethers
├── README.md              # Project documentation
├── report.pdf             # Detailed report of the simulations
├── requirements.txt       # Python dependencies for analysis
├── figs/                  # Directory containing generated figures
│   ├── 3d_density_1_vs_2.png
│   ├── 3d_density_1_vs_4.png
│   ├── ...
```

## How to Compile and Run

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/YagizEbil/cyclohexane_namd_simulation.git
   cd cyclohexane_namd_simulation
   ```

2. **Install Dependencies**:
   Install the required Python libraries for analysis:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Simulations**:
   Use the cyclohexane.namd configuration file to run simulations with NAMD:
   ```bash
   namd2 cyclohexane.namd > output.log
   ```

4. **Analyze Results**:
   Open the Jupyter notebook main.ipynb to analyze and visualize the simulation results:
   ```bash
   jupyter notebook main.ipynb
   ```

5. **View Figures**:
   Already generated figures are stored in the figs directory for density and PMF visualizations and many more.

## Authors

- [Kadir Yağız Ebil](https://github.com/YagizEbil)

## License

This project is licensed under the MIT License. Built for molecular dynamics simulations and analysis.