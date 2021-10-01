# LigParGen2Mol.jl

Convert LAMMPS data files generated by LigParGen into molecule description and
pair/bond/angle/dihedral/improper coeffs section for LAMMPS.

Usage:

    write_mol(f, ligpargenfile::AbstractString)

Read the molecular topology from file named `ligpargenfile` and write it into `f`. `f` can
    be an I/O stream or a filename.

    write_ff(f, ligpargenfile::AbstractString)

Read the molecular topology from file named `ligpargenfile` and write its forcefield
    into `f`. `f` can be an I/O stream or a filename.

    write_ff(f, ligpargenfile::AbstractString)

Read the molecular topology and forcefield parameters from `ligpargenfile` and write them
    into files "fmask.txt" and "fmask.ff", respectively.
