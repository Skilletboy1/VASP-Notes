# KPOINT generation using VASPKIT
## Required Files
> POSCAR

> POTCAR
## Steps
1. vaspkit
2. 1
3. 102
4. [1. Monkhorst-Pack Scheme] [2. Gamma Scheme]
5. Input accuracy
6. INCAR and KPOINTS will be written

## Gamma vs Monkhorst-Pack
### Gamma
Centers the KPOINT  grid right at the gamma point which is the origin of reciprocal space. Good for systems where fewer KPOINTS are needed, so bigger systems. 

### Monkhorst-Pack
Also gives a grid of KPOINTS, however does so such that it is symmetric, regardless of whether it includes the gamma point. Better for smaller systems where more KPOINTS are used. Samples the Brillouin zone more uniformly.

## ONLY USED FOR SCF CALCULATIONS