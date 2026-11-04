# PKD2_Function_In_Pi

Simulation inputs, analysis notebooks and representative structures for the paper "TRPP Ion Channels Function in the π-Conformation Rather Than the α-Conformation" by Chenfeng Zhang, Wojciech Kopec and Julien Michel.

Systems follow Supplementary Table S1 and simulation sets follow Supplementary Table S2.

Trajectories supporting the main conclusions, with a reduced number of frames, are available on Zenodo (https://doi.org/10.5281/zenodo.23946105).

## Layout

```
01_systems/          simulation boxes, split by force field
  CHARMM/            CHARMM36m + CHARMM-modified TIP3P
  OPC/               AMBER ff19SB + OPC + 12-6-4 ions
    NN_<system>/     step5_input.gro, index.ndx, topol*.top and toppar*/
02_simulations/      GROMACS .mdp and PLUMED input files, split by force field
  CHARMM/
  OPC/
03_scripts/          analysis notebooks
  pore_hydration.ipynb   water density along the pore axis
  permeation.ipynb       ion permeation events and conductance
  trp_survey.ipynb       lower-gate survey of TRP channel cryo-EM structures
04_snapshots/        representative structures shown in the figures
```