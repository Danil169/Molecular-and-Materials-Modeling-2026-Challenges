=====================================================
Challenge I.4: Testing MACE Installation
=====================================================

Objective
---------
Run all testing scripts for the MACE machine-learning interatomic potential using ASE
and verify geometric relaxation behavior.

Results
-------
* Geometry optimization of H₂O performed using both EMT and MACE-MP-0 calculators.
* Both calculators converged to minimum energy geometries without errors.
* Output trajectories saved as ``water_opt_emt.traj`` and ``water_opt_mace.traj``.

Files in this Directory
-----------------------
* ``water_opt.py``: Relaxation test script using ASE + MACE.
* ``water_opt.log``: Convergence log.
* ``*.traj``: Trajectory files verifying successful runs.
