=====================================================
Challenge I.3: Diatomics Atomization Energies
=====================================================

Objective
---------
Modify the ASE script to compute atomization energies of diatomic molecules (N₂, O₂)
comparing the classical Effective Medium Theory (EMT) and the MACE-MP-0 machine learning potential.

Results
-------
* **N₂ molecule**:
  * EMT Atomization Energy: 9.76 eV
  * MACE Atomization Energy: 9.88 eV
  * Experimental benchmark: 9.79 eV (excellent agreement)
* **O₂ molecule**:
  * Evaluated with triplet spin state consideration.
* **Physical Insights**:
  * EMT is parameter-limited and lacks coverage for certain elements (e.g., F₂).
  * MACE provides wide elemental coverage but exhibits residual self-interaction error for highly electronegative bonds.

Files in this Directory
-----------------------
* ``diatomics_atomization_EMT_MACE.py``: Script computing atomization energies for N₂ and O₂.
* ``diatomics_atomization.log``: Execution output and energy table.
