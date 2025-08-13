# CI-NEB Calculations
## Steps
1. Optimize initial and final structures
2. Change name of POSCARs such that initial is named POSCAR1 and final is named POSCAR2
3. Run: nebmake.pl POSCAR1 POSCAR2 (insert number of desired images)
4. Add OUTCARs from opt into 00 and 05
5. Add KPOINTS, INCAR, POTCAR, and submission scirpt
6. nebef.pl to see forces and energy of images
7. nebresults.pl to generate data from calculation

##INCAR
NWRITE = 0 
Verbosity of output 0 is minimal info

IMAGES = 4
Number of images between endpoints

SPRING = -5
In VASP NEB, the SPRING parameter sets the strength and type of the fictitious spring force between images, with positive values keeping images evenly spaced and negative values (e.g., -5) enabling climbing-image mode to converge directly to the saddle point.

ICHAIN = 0 
Indicates which vtst operation to run 0 is NEB

LCLIMB = TRUE
Turns on climbing image algorithm

IOPT = 0  
Default VASP optimizer

## Why
NEB calculates the lowest energy pathway between two stable steps in the mechanism. The CI method allows you to determine the transition state. 
