# How to make an INCAR for a DFT+U Calculations
## DFT+U Paramters for SACs (C, N, Sc)
LDAU = .TRUE.               
Turns on DFT+U

LDAUTYPE = 2                
Simplified approach to DFT+U

LADAUL = -1 -1 2            
1-quantum number (-1: no U, 1: p group, 2: d group, 3:f group) (angular quantum number: s=0, p=1, d=2, f=3, g=4)

LDAUU = 0.0 0.0 2.11      
U correction value

LDAUJ = 0.0 0.0 0.0         
J for Hund's exchange paramter, accounts for intra-atomic exchange interactions. Generally people just put at 0 and use an effective U and put it in LDAUU

LMAXMIX = 4          
Represents the non-spherical contributions, essentially VASP considers the other orbital shapes. So it takes the angular quantum number and tells VASP what shapes to consider. So in the case of Sc, 4 since it is a d-metal

LDAUPRINT = 2
0: Silent, 1: Write occupancy matrix to OUTCAR, 2: 1+ potential matrix

LASPH = .TRUE. 
Tells VASP to consider non speherical electron cloud shapes