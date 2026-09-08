=====================================================
Challenge II.6: Graphene 2D Modeling & Dirac Cone
=====================================================

Objective
---------
Construct monolayer graphene in a 15 Å vacuum slab, run 2D convergence tests, execute
constrained cell relaxation (in-plane xy only), and decompose projected DOS into px, py, and pz.

Results
-------
1. **2D Convergence**:

   * Cutoff converged at **100 Ry** (Carbon 2p hard pseudopotential).
   * K-point grid: **(42, 42, 1)** (Extremely dense to sample the Dirac point at K).

2. **K-Grid DOS Comparison**:

   * DOS was calculated and compared for **k=12, 18, and 20** meshes.
   * Lower k-point densities show artificial jaggedness and gaps near the Fermi level due to poor sampling of the linear dispersion.
   * Higher k-point density (e.g. k=42) is necessary for a perfectly smooth DOS that reaches exactly zero at the Dirac point.

3. **Constrained Relaxation**:

   * UnitCellFilter mask ``[True, True, False, False, False, False]`` preserves vacuum.
   * Relaxed C-C bond length: **1.424 Å** (Exp: 1.420 Å, 99.7% match).
   * Relaxed lattice constant: **a = 2.466 Å** (Exp: 2.460 Å).

4. **Orbital Decomposition & Dirac Cone Physics**:

   * In-plane **px** and **py** orbitals form strong, deep σ-bonds far below Fermi level.
   * Out-of-plane **pz** orbital exclusively forms the electronic states crossing the
     Fermi level, creating the iconic linearly dispersing Dirac cone.


Files in this Directory
-----------------------
* ``k12/``, ``k18/``, ``k20/``: Subdirectories containing DOS data for different k-grids showing convergence behavior.
* ``convergence_test_graphene.py``: 2D convergence sweep script.
* ``cell_relaxation_graphene.py``: Constrained in-plane relaxation script.
* ``electronic_properties_graphene.py``: SCF + NSCF + projwfc.x pipeline.
* ``Graphene_PDOS.png``: Plot showing pz dominance at the Dirac point.
* ``Graphene_Total_p_PDOS.png``: Total p-orbital contribution.
* ``final_relaxed_structure.vasp``: Final relaxed 2D coordinates.
