=====================================================
Challenge I.7: QE Geometry Relaxation of Methane (CH₄)
=====================================================

Objective
---------
Adapt the Quantum ESPRESSO water-relaxation script to perform ab-initio geometry
optimization of methane (CH₄) inside a periodic vacuum box.

Computational Details
---------------------
* Functional: PBE GGA
* Plane-wave cutoff: ``ecutwfc = 46 Ry``
* Brillouin zone: Gamma point only (isolated molecule in 12 Å cubic box)
* Optimizer: ASE BFGS with Quantum ESPRESSO calculator

Results
-------
* **Total Energy**: **-315.702 eV**
* **Mean C-H bond length**: **1.0957 Å** (Exp: 1.087 Å, deviation 0.8%)
* **H-C-H bond angle**: **109.47°** (Perfect tetrahedral symmetry)
* **Max residual force**: **0.006 eV/Å** (< 0.01 eV/Å threshold)

Files in this Directory
-----------------------
* ``relax_ch4_qe.py``: ASE-driven Quantum ESPRESSO relaxation script.
* ``relax_ch4_qe.out``: Full calculation stdout.
* ``ch4_relax.log``: BFGS optimization steps.
* ``ch4_final.xyz``: Final relaxed Cartesian coordinates.
* ``espresso.pwi``, ``espresso.pwo``: QE input card and output log.
