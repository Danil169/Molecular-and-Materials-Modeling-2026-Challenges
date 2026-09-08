=====================================================
Challenge I.8: UO₂I₂(OH₂)₂ Optimization with MACE & NWChem
=====================================================

Objective
---------
Perform multi-scale structural modeling of the actinide complex UO₂I₂(OH₂)₂ combining
MACE machine-learning potential pre-optimization and NWChem scalar-relativistic DFT.

Results
-------
* Pre-optimization using MACE rapidly produced a reasonable coordination geometry.
* NWChem refinement using B3LYP with Stuttgart relativistic effective core potentials (ECP)
  for Uranium converged to the energy minimum.
* All output files and coordinates preserved for verification.

Files in this Directory
-----------------------
* ``mace/uo2i2_core_mace-geopt.py``: MACE pre-optimization script.
* ``mace/uo2i2_initial.xyz``: Initial coordinate file.
* ``nwchem/uo2i2water2_b3lyp_stuttgart_rlc_ecp.nw``: NWChem input deck.
* ``nwchem/uo2i2water2_b3lyp_stuttgart_rlc_ecp.nw_logfileSAVED_VictusNB_N4``: NWChem calculation log.
* ``nwchem/geopt/``: Geometry optimization step files and final coordinates.
