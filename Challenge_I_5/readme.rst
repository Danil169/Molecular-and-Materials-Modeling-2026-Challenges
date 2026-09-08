=====================================================
Challenge I.5: Thermodynamic Properties of Diatomics
=====================================================

Objective
---------
Modify the ASE IdealGasThermo script to compute thermodynamic properties (entropy,
enthalpy, free energy) of O₂ in its triplet ground state.

Results
-------
* **Spin state**: Open-shell triplet (multiplicity = 3, ``spin=1`` in ASE).
* **Calculated Entropy S° (298.15 K)**: **205.2 J/(mol·K)**.
* **Experimental benchmark (NIST)**: **205.15 J/(mol·K)**.
* **Agreement**: **99.98% match**! Correct specification of electronic degeneracy
  is essential for reproducing experimental gas-phase entropy.

Files in this Directory
-----------------------
* ``O2_thermodyn_EMT_MACE.py``: Script setting up vibration analysis and IdealGasThermo.
* ``O2_thermodyn_EMT_MACE.py_logfileSAVED``: Output log with full thermochemical table.
* ``vib_o2_mace/``: Hessian displacement caches.
