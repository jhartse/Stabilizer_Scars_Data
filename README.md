# Stabilizer_Scars_Data
Raw data for "Stabilizer Scars" by J. Hartse, L. Fidkowski, and N. Mueller

The "Entanglement" folder has all the raw data for the entanglement components. The subfolders are "Z2" for the Z2 lattice gauge theory data and "Ising" for the dual ising data. Each of these two subfolders have the subfolders are "Odd" for the odd length lattice data, "Even" for the even length lattice data. The sub-folders in these are named for the parameters:

    N - the symmetry group ZN (mostly N = 2 for this data)
    NxA - the length of the subregion of the lattice that the entanglement is calculated off of
    NxB - the length of the corresponding other subregion. Total length of the lattice is L = NxA + NxB
    Ny - the height of the lattice (mostly 2 for this data)
    K0 - the plaquette coupling 
    g0 - the electric coupling
    eps_x - the electric coupling (for the ising data)
    
The entanglement data is is stored in "entang.bin" in each of these folders. "entang.bin" is a 3 by 2^(2L-1) array. The first column is the energy, the second column is the symmetry entanglement component, and the third column is the distillable entanglement component. The rows correspond to the energy eigenstates.  

The "Time_evo" folder contains the raw data for the time evolution plots. There is a subfolder called "Observables" for the observable measurement data. There is another subfolder called "Echo" that contains the loschmidt echo data, with subfolders "Scar" and "Non-scar" that has the data for a scar and non-scar respectively. There is another subfolder called "Entanglement" which has the entanglement time evolution data. And the last subfolder is called "Random_circuit" that has loschmidt echo data from the random time evolution circuit. The subfolders in all of these are named for their parameters (see above), including the new parameters:
    
    time - the length of time that the state is evolved for
    dt - the size of the timestep
    g_quench - the coupling used for the time evolution
    steps - the number of steps in the random circuit

The loschmidt echo data is stored in "echo_scar.bin" and "echo_nonscar.bin" respectively. The entanglement data is stored in "entang_nonscar". The observables data is stored in files named like "X_plaq_scar" that describe what observables are measured. 
    
