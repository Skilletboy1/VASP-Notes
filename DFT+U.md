# DFT+U Calculations
## What is it
>> DFT with VanDerWaal Corrections

## INCAR
>> IVDW = 11 DFT-D3 Method of Grimme

>> LDAU = .TRUE. Switches on DFT+U

>> LDAUL = -1 3 -1:No U, 2:d group metals, 3:f group metals POSCAR has O and Ce. O has no U, Ce is a f group metals

>> LDAUU = 0.0 5.0 fro Ce:5.0 and O: O (U values (eV))

>> LDAUJ = 0.0 0.0 J values (For LADAUTYPE=2, Ueff=U-J) [Here the J values are already calculated in to the LDAUU]

>>LMAXMIX = 6 4 for d electrons, 6 for f-electrons

>> LDAUPRINT = 2 0: silent, 1: Write occupancy matrix to OUTCAR, 2: 1+ potential matrix

>> LASPH = .TRUE.  non-spherical contributions from the gradient corrections inside the PAW spheres will be
