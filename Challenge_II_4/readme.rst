=====================================================
Challenge II.4: Effect of Gaussian Broadening (degauss)
=====================================================

Objective
---------
Investigate the effect of Gaussian smearing parameter (``degauss`` = 0.005, 0.010, 0.020 Ry)
on the total energy and density of states (DOS) of semiconducting silicon.

Results
-------
* **Total Energy**:
  * degauss = 0.005 Ry: **-230.280072 eV**
  * degauss = 0.010 Ry: **-230.280072 eV**
  * degauss = 0.020 Ry: **-230.280072 eV**
  * Total energy is completely invariant to smearing in semiconductors (gap > 0).
* **DOS at Fermi Level**:
  * degauss = 0.005 Ry: **0.000000 states/eV** (Pure gap)
  * degauss = 0.010 Ry: **0.000102 states/eV** (Tiny tail)
  * degauss = 0.020 Ry: **0.012140 states/eV** (Artificial smearing into the gap)
* **Conclusion**: For semiconductors, small degauss values (<= 0.01 Ry) or tetrahedron
  integration are necessary to avoid smearing states artificially into the band gap.

Files in this Directory
-----------------------
* ``compare_degauss.py``: Automation script testing multiple broadening parameters.
* ``compare_degauss.out``: Execution output.
* ``degauss_summary.csv``: Quantitative comparison table.
* ``dos_dg*.dat``: Calculated DOS datasets for each degauss value.
