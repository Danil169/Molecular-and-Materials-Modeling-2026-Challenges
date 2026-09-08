=====================================================
Challenge I.6: C-H Bond Dissociation Energy in Methane
=====================================================

Objective
---------
Modify the ethane C-C bond energy script to compute the C-H bond dissociation energy in
methane (CH₄ → CH₃ + H) using ASE with EMT and MACE.

Results
-------
* **MACE C-H Bond Energy**: **4.48 eV** (432.2 kJ/mol).
* **Experimental value**: **4.54 eV** (438 kJ/mol) — excellent agreement (< 1.5% error).
* Trajectories for CH₄, CH₃, and isolated H relaxation converged smoothly.

Files in this Directory
-----------------------
* ``methane_CH_bond_en_EMT_MACE.py``: Script calculating methane C-H bond cleavage.
* ``methane_CH_bond_en_EMT_MACE.out``: Output log.
* ``Methane_CH_Bond_Report.docx``: Standalone detailed report for this challenge.
* ``*.traj``: Relaxation trajectory files.
