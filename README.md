# CHARMM_secondary_structure
FORTRAN code for introducing secondary structure biasing potentials to CHARMM code.

## How to compile a new CHARMM forcefield
* modify F_BETA_NAUGHT and K_CONST in usersb.src (L114 and L115)
* replace your CHARMM source code's usersb.src file (usually at source/charmm/usersb.src) with the modified one
* recompile CHARMM source code to run in parallel (using MPI) with the following command:
** ./install.com gnu xxlarge M MPIF90 X86_64


