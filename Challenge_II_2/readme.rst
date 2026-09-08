=====================================================
Challenge II.2: Si Forces, Stress & Pseudopotentials
=====================================================

Objective
---------
1. Run final SCF calculation on Si unit cell using fully converged parameters (65 Ry,
   15x15x15 k-grid) with ``tstress = .true.`` and ``tprnfor = .true.``.
2. Compare convergence behavior across different silicon pseudopotentials.

Results
-------
1. **Force & Stress on unrelaxed experimental cell**:
   * Total Energy: **-16.92488372 Ry**
   * Forces on both Si atoms: **0.000000 Ry/Bohr** (Zero due to inversion symmetry)
   * Hydrostatic Stress/Pressure: Non-zero, driving cell expansion during relaxation.
2. **Pseudopotential comparison**:
   * Norm-conserving pseudopotentials require ~65 Ry cutoff.
   * Ultrasoft and PAW potentials achieve comparable convergence around 35-45 Ry.
   * Full data recorded in ``si_pseudopotential_convergence.csv``.

Files in this Directory
-----------------------
* ``Si_force_stress.in``, ``Si_force_stress.out``: QE input card and output with stress tensor.
* ``compare_si_pseudopotentials.py``: Automation script comparing pseudopotentials.
* ``si_pseudopotential_convergence.csv``: Benchmark comparison data.
