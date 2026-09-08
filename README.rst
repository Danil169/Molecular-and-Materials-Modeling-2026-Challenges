====================================================================
Solved Challenges: Molecular and Materials Modeling School (2026)
====================================================================

**Student:** Danil  
**Instructors:** Miroslav Iliaš and Dipayan Sen (BLTP JINR, Dubna)  
**School Date:** August 26–27, 2026  
**Repository:** https://github.com/Danil169/Molecular-and-Materials-Modeling-2026-Challenges

Overview
========

This repository contains the standalone, fully solved challenge exercises for the
*Two-Day Hybrid School on Molecular and Materials Modeling*. Per instructor instructions,
this repository contains **only the solved challenges**, organized into dedicated directories
with descriptive ``readme.rst`` files, inputs, scripts, logs, outputs, and generated figures.

Comprehensive Final Reports
===========================

* **`Report_Materials_Modeling_EN.docx <Report_Materials_Modeling_EN.docx>`_**:
  Full English technical report containing detailed methodologies, numerical tables, and
  eight embedded figures. (Verified 100% valid OpenXML).
* **`Report_Materials_Modeling_EN.pdf <Report_Materials_Modeling_EN.pdf>`_**:
  Directly viewable PDF version of the English report.

Directory Structure & Solved Challenges
=======================================

Part I: Molecular Modeling
--------------------------

* **`Challenge_I_1/ <Challenge_I_1/readme.rst>`_**: Basic software functionality tests
  (PySCF: -2067.61 eV, MOPAC: -2.50 eV, xTB: -137.97 eV, CREST, NWChem, Quantum ESPRESSO).
* **`Challenge_I_2/ <Challenge_I_2/readme.rst>`_**: Multi-core performance benchmarks
  (MOPAC scaling 1–24 threads, QE MPI scaling, NWChem MPI).
* **`Challenge_I_3/ <Challenge_I_3/readme.rst>`_**: Diatomics atomization energies (N₂, O₂)
  comparing EMT and MACE-MP-0 MLIP.
* **`Challenge_I_4/ <Challenge_I_4/readme.rst>`_**: MACE installation testing and water
  relaxation verification.
* **`Challenge_I_5/ <Challenge_I_5/readme.rst>`_**: Gas-phase thermodynamic properties of triplet O₂
  (S° = 205.2 J/(mol·K), 99.98% match with NIST experiment).
* **`Challenge_I_6/ <Challenge_I_6/readme.rst>`_**: C–H bond dissociation energy in methane
  (MACE: 4.32 eV vs Exp: 4.54 eV; includes dedicated DOCX report).
* **`Challenge_I_7/ <Challenge_I_7/readme.rst>`_**: QE/ASE ab-initio geometry relaxation of methane
  (C–H = 1.096 Å, H–C–H = 109.47° tetrahedral).
* **`Challenge_I_8/ <Challenge_I_8/readme.rst>`_**: Multi-scale modeling of actinide complex
  UO₂I₂(OH₂)₂ with MACE pre-optimization and NWChem relativistic DFT.

Part II: Materials Modeling
---------------------------

* **`Challenge_II_1/ <Challenge_II_1/readme.rst>`_**: Silicon unit cell energy cutoff convergence
  (20–80 Ry sweep, monotonic convergence to basis set limit).
* **`Challenge_II_2/ <Challenge_II_2/readme.rst>`_**: Si converged force/stress calculations
  and pseudopotential comparison (norm-conserving vs USPP/PAW).
* **`Challenge_II_3/ <Challenge_II_3/readme.rst>`_**: Tight cell relaxation with shifted atomic positions
  (restoring ideal diamond lattice, a = 5.468 Å).
* **`Challenge_II_4/ <Challenge_II_4/readme.rst>`_**: Effect of Gaussian broadening (degauss) on Si DOS
  (demonstrating artificial gap-smearing at degauss > 0.01 Ry).
* **`Challenge_II_5/ <Challenge_II_5/readme.rst>`_**: Complete Aluminum pipeline from experimental structure
  (cutoff/k-point convergence, 0 K cell relaxation to a = 4.038 Å, metallic continuous DOS).
* **`Challenge_II_6/ <Challenge_II_6/readme.rst>`_**: Monolayer Graphene 2D constrained relaxation
  (C–C = 1.424 Å) and orbital-resolved PDOS proving pz-derived Dirac cone.
* **`Challenge_II_7/ <Challenge_II_7/readme.rst>`_**: Graphene work function determination (4.24 eV)
  and physical evaluation of the ``'assume_isolated': '2D'`` flag.
* **`Challenge_II_8/ <Challenge_II_8/readme.rst>`_**: Surface adsorption: H on C8 (high cutoff 100 Ry)
  and extended modeling of Mercury (Hg) on C18 graphene flake.

Summary Table
=============

+--------------------+-------------+---------------------------------------+-------------+
| Challenge          | Category    | Key Result                            | Status      |
+====================+=============+=======================================+=============+
| Challenge I.1      | Molecular   | All packages verified (PySCF, etc.)   | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.2      | Molecular   | Benchmark scaling 1 to 24 cores       | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.3      | Molecular   | N₂ atomization: 10.31 eV (MACE)       | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.4      | Molecular   | MACE relaxation tests passed          | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.5      | Molecular   | O₂ triplet S° = 205.2 J/(mol·K)       | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.6      | Molecular   | Methane C–H: 4.32 eV (Exp: 4.54 eV)   | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.7      | Molecular   | CH₄ QE relaxation: 109.47° tetrahedral| Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge I.8      | Molecular   | UO₂I₂(OH₂)₂ MACE + NWChem DFT         | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.1     | Materials   | Si cutoff converged at 65 Ry          | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.2     | Materials   | Si stress & pseudopotential benchmark | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.3     | Materials   | Tight relaxation: a = 5.468 Å         | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.4     | Materials   | degauss effect: gap preservation      | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.5     | Materials   | Al metal pipeline: continuous DOS     | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.6     | Materials   | Graphene Dirac cone from pz orbital   | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.7     | Materials   | Graphene Work Function: W = 4.241 eV  | Completed   |
+--------------------+-------------+---------------------------------------+-------------+
| Challenge II.8     | Materials   | H@C8 (2.86 eV) & Hg@C18 (-7481 eV)    | Completed   |
+--------------------+-------------+---------------------------------------+-------------+

Reproducibility
===============

All calculations can be inspected via the provided output logs, structures, and scripts.
No recalculations are required.
