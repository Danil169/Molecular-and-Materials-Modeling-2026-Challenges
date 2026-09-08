=====================================================
Challenge II.7: Graphene Work Function & Isolation Flag
=====================================================

Objective
---------
Calculate the work function of graphene (W = Evac - EF) and evaluate the effect of the
``'assume_isolated': '2D'`` flag on the electrostatic potential profile.

Results
-------
1. **Work Function Determination**:
   * With 2D flag: **W = 4.241 eV** (EF = -4.241 eV, Evac = +0.001 eV)
   * Without 2D flag: **W = 4.237 eV** (EF = -1.717 eV, Evac = +2.520 eV)
   * Both values agree within **0.004 eV** and match experimental graphene (4.2-4.5 eV).
2. **Electrostatic Potential Profile**:
   * The ``'assume_isolated': '2D'`` flag introduces artificial dipole image charges at
     the periodic boundaries, producing sharp unphysical spikes near the cell edges.
   * Removing the flag yields a smooth, flat, physically meaningful vacuum plateau.

Files in this Directory
-----------------------
* ``compare_isolation.py``: Script comparing electrostatic potential with and without 2D flag.
* ``compare_isolation.out``: Numerical comparison log.
* ``isolation_summary.csv``: Quantitative summary table.
* ``avg_2d.dat``, ``avg_none.dat``: Planar and macroscopic averaged potential datasets.
* ``potential_plot_python.png``: Full work function potential diagram.
