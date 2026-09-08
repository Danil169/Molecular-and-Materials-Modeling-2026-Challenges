=====================================================
Challenge II.1: Si Unit Cell Cutoff Convergence Test
=====================================================

Objective
---------
Investigate the energy convergence of the diamond silicon unit cell with respect to the
plane-wave energy cutoff (``ecutwfc``) from 20 to 80 Ry.

Results
-------
* Direct QE SCF: **E = -16.736497 Ry** (-227.711622 eV).
* ASE-driven QE: **E = -227.711622 eV**.
* Energy convergence demonstrates monotonic asymptotic approach to the basis-set limit:
  * 20 Ry: -227.684 eV
  * 40 Ry: -227.710 eV
  * 60 Ry: -227.712 eV
  * 80 Ry: -227.712 eV (Fully converged, ΔE < 0.001 eV)

Files in this Directory
-----------------------
* ``ecutwfc_test.py``: Standalone ASE script evaluating cutoff convergence.
* ``Si.out``: Direct QE reference output.
* ``si_ase.out``: ASE execution output.
* ``espresso.pwo``: QE log confirming ``JOB DONE``.
