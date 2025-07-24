# Density of States Notes
## Input Files
### INCAR
#### Regular Paramters
>>  -ISYM=0 Symmetry is switched off

#### Include Mangetization Parameters

>>-LORBIT=11 Gets magneization density

>>-MAGMOM to get magnetic moment for each atom

#### DOS Paramters

>>-LORBIT=11

>>-EMIN=-12 Minimum energy (in eV) for the DOS window

>>-EMAX=2 Maximum energy (in eV) for the DOS window

>>-NEDOS=5000 Number of energy grid points


### KPOINTS
>>    -Can also be generated through VASPKIT
### POSCAR
>>    -Entirely dependent on system
### POTCAR
>>    -A fairly standard POTCAR

>>    -Can be generated using VASPKIT and a POSCAR

## Output Files
### DOSCAR
>>    -Most important output file

## VASPKIT
>>    -Use VASPKIT to generate the various DOS graph datas
>>    -Then using a plotting software, build out the plots


## Purpose
#### Density of state is highly important to catalytic studies as it reveals the root causes for bonding and bond strength. This allows one to gain a mechanistic understanding of all aspects of a good catalyst. Including stability, activity, selectivty. 


