### This repository contains the necessary topology, structure, gromacs parameter and plumed files to run MEMMI in an IAPP fibril system

__To run MEMMI first you need to install the relevant PLUMED version:__ 
1. git clone https://github.com/tlhr/plumed2.git plumed2
2. cd plumed2
3. git checkout emmi-bias-sem

__TOPO_MDP__ folder contains GROMACS topology and parameter files.
PRODUCTION containst the plumed file and the associated companion files such as an index file, data GMM file (iapp.dat),  structure.pdb file and job submission file used.

__PRODUCTION_TPR__ contains the folders containing the .tpr files of each replica. Uppon simulation the r$i foders should be contained in the PRODUCTION folder. 

__ANALYSIS__ folder contains the plumed_analysis.dat file used to print the CVs of the biased N-tail side as well as the final torrie-value weight per-frame. plumed_analysis_unbiased.dat is used to print the unbiased N-tail side CVs. plumed_error.dat to write the Overlap files per frame

__MEMMI_IAPP_example.ipynb__: contains steps to do the analysis (FES, error estimate, local correlation, reampling of the structural ensemble) of MEMMI 

__Samples  of the ensemble__ without protein-hydrogens or water/ions can be found in Zenobo https://zenodo.org/record/6518554#.YnLwby8Rqhw

__References__

 Z. F. Brotzakis, T. Löhr, S. Truong, S. E. Hoff, M. Bonomi and M. Vendruscolo Determination of the
structure and dynamics of the fuzzy coat of an amyloid fibril of IAPP using cryo-electron microscopy.
Biochemistry 2023, 62, 16, 2407–2416 (doi: 10.1021/acs.biochem.3c00010)




