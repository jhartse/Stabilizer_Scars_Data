# Stabilizer_Scars_Data
Raw data for "Stabilizer Scars" by J. Hartse, L. Fidkowski, and N. Mueller

The "Entanglement" folder has all the raw data for the entanglement components. The subfolders are "Odd" for the odd length lattice data, "Even" for the even length lattice data, and "Ising" for the dual ising data. The sub-folders in these are named for the parameters:
    N - the symmetry group ZN (mostly N = 2 for this data)
    NxA - the length of the subregion of the lattice that the entanglement is calculated off of
    NxB - the length of the corresponding other subregion. Total length of the lattice is L = NxA + NxB
    Ny - the height of the lattice (mostly 2 for this data)
    K0 - the plaquette coupling 
    g0 - the electric coupling
    eps_x - the electric coupling (for the ising data)
The entanglement data is is stored in "entang.bin" in each of these folders. "entang.bin" is a 3 by 2^(2L-1) array. The first column is the energy, the second column is the symmetry entanglement component, and the third column is the distillable entanglement component. The rows correspond to the energy eigenstates.  

The "time_evo" folder contains the raw data for the 
