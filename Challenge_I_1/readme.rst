=====================================================
Challenge I.1: Basic Software Functionality Tests
=====================================================

Objective
---------
Run scripts for basic software functionality tests across all required computational
chemistry packages: PySCF, MOPAC, xTB, CREST, NWChem, and Quantum ESPRESSO.

Results & Confirmation
----------------------
All packages were verified on the local Linux workstation:

* **PySCF**: Single-point SCF energy of small test molecule: **E = -2067.61 eV** (Job completed successfully).
* **MOPAC (PM7)**: Semiempirical SCF energy: **E = -2.50 eV** (Outputs: ``mopac.out``, ``mopac.arc``).
* **xTB (GFN2-xTB)**: Tight-binding calculation: **E = -137.97 eV** (Output: ``xtbtopo.mol``).
* **CREST**: Conformer generation and search successfully executed.
* **NWChem**: DFT energy calculation completed successfully (Outputs: ``tmp_nwchem.*``).
* **Quantum ESPRESSO**: Plane-wave self-consistent field calculation completed (``JOB DONE``).

Files in this Directory
-----------------------
* ``mopac.mop``, ``mopac.out``, ``mopac.arc``: MOPAC input and output files.
* ``tmp_nwchem.*``: NWChem calculation database and output artifacts.
* ``xtbtopo.mol``: xTB molecular topology output.
