=====================================================
Challenge II.5: Aluminum Complete Modeling Pipeline
=====================================================

Objective
---------
Take experimental FCC aluminum structure (a = 4.049 Å), run convergence tests (cutoff and
k-points), perform cell relaxation, and recalculate electronic properties (DOS).

Results
-------
1. **Convergence Testing (1_convergence_al.py)**:

   * Cutoff converged at **50 Ry**.
   * K-points show characteristic metallic oscillations due to Fermi surface integration,
     requiring dense sampling (12x12x12).

2. **Cell Relaxation (2_relax_al.py)**:

   * Relaxed lattice vector: **2.019158 Å** (a = 4.0383 Å).
   * Slight contraction from experimental room-temperature value (4.049 Å) correctly reflects
     0 K DFT ground state (no thermal expansion).
   * Residual force: **f_max = 0.000470 eV/Å**.

3. **Electronic Properties (3_electronic_al.py)**:

   * High-density NSCF calculation (24x24x24 k-grid).
   * DOS intersects Fermi level continuously (no band gap) — clear metallic signature.


Files in this Directory
-----------------------
* ``1_convergence_al.py``: Cutoff and k-point convergence script.
* ``2_relax_al.py``: BFGS cell relaxation script.
* ``3_electronic_al.py``: High-resolution SCF + NSCF DOS calculation script.
* ``al_relaxed.vasp``: Relaxed structure POSCAR.
* ``al_total_dos.dat``: Final computed DOS dataset.
* ``Al_DOS.png``: Density of states plot showing metallic character.
