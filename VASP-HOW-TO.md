# How to Setup a VASP Calculations
## Files Needed
### INCAR
> Sets up the parameters of the calculation. Sort of like the settings of the calculations
### POSCAR
> Creates the atomic system that the calculations is to be run off. Includes the atoms, and their respective positions.
### POTCAR
> Contains the information of the pseudopotentials needed to conduct the calculations.
### KPOINTS
> Method in which to simplify calculations. Electrons act like waves and can be described by a wavevectors K. So, pick a number of kpoints to calculate with. The higher the number, the greater the accuracy, but the more computationally intensive.
### Submission Script
> Essentially just tells the cluster how to run the calculation. What version of vasp is being run, how much RAM, cores, and etc should be allocated. 
