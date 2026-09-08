=====================================================
Challenge II.3: Tight Cell Relaxation with Shifted Atoms
=====================================================

Objective
---------
Subject the Si diamond lattice to artificial initial atomic displacements (breaking
symmetry) and perform variable-cell relaxation with strict force (1e-4 Ry/Bohr) and energy
(1e-5 Ry) convergence thresholds.

Results
-------
* Both direct QE (``vc-relax``) and ASE BFGS optimizations successfully restored the
  perfect diamond tetrahedral coordinates.
* Final relaxed lattice constant: **a = 5.468 Å** (a/√2 = 2.734 Å).
* Final residual force: **f_max < 0.001 eV/Å**.

Files in this Directory
-----------------------
* ``si_vc_relax_tight.in``, ``si_vc_relax_tight.out``: Direct QE tight relaxation input and log.
* ``relax_si_tight_ase.py``: ASE optimization script with shifted coordinates.
* ``si_tight_ase.log``: BFGS optimization trajectory log.
* ``si_tight_ase_final.vasp``: Final relaxed VASP POSCAR structure.
