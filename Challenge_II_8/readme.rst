========================================================
Challenge II.8: Surface Adsorption (H on C8 & Hg on C18)
========================================================

Objective
---------
1. Perform relaxation of the C8 graphene flake and recalculate H adsorption binding energy
   at high cutoff (100 Ry).
2. Extended Challenge: Model adsorption of heavy metal Mercury (Hg) on an expanded C18 flake
   at multiple adsorption sites (top, bridge, hollow) to find the most stable configuration.

Results
-------
1. **H on C8 Adsorption**:

   * E(H@C8) relaxed: **-1319.069 eV**
   * E(H) isolated: **-12.560 eV**
   * E(C8) clean: **-1303.646 eV**
   * Calculated Binding Energy: **E_bind = 2.864 eV**
   * Increasing cutoff to 100 Ry confirms energetic convergence. Small finite flake
     exhibits edge-induced enhanced binding compared to infinite graphene (~0.7-1.0 eV).

2. **Extended Challenge: Hg on C18**:

   * Adsorption of Mercury on the larger C18 graphene flake was modeled for three high-symmetry sites.
   * **Top site** is the most stable configuration with the lowest energy.
   * **Bridge** and **Hollow** sites showed weaker binding or relaxation towards the top site.
   * BFGS relaxation converged smoothly for the lowest energy state (f_max < 0.01 eV/Å).
   * Relaxed total energy: **-7481.346 eV**.

Files in this Directory
-----------------------
* ``relax_c8_highcutoff.py``: High-cutoff C8 and H@C8 relaxation script.
* ``relax_c8_highcutoff.out``: Optimization log.
* ``c8_100Ry_final.vasp``, ``hc8_100Ry_final.vasp``: Relaxed geometries.
* ``Hg_on_C18/``: Dedicated workspace for Mercury adsorption on C18 flake.
