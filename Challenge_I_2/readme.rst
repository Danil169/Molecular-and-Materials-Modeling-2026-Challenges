=====================================================
Challenge I.2: Software Performance Benchmarks
=====================================================

Objective
---------
Run NWChem, Quantum ESPRESSO, and MOPAC performance tests across various CPU core counts
(1 to 24 cores) on an Intel Core i9-14900KF processor.

Results & Observations
----------------------
1. **MOPAC (DNA PM7 calculation)**:
   * 1 thread:  48.2 s
   * 2 threads: 27.1 s (Speedup: 1.78x)
   * 4 threads: 16.4 s (Speedup: 2.94x)
   * 8 threads: 11.2 s (Speedup: 4.30x)
   * 16 threads: 9.1 s (Speedup: 5.30x)
   * 24 threads: 8.8 s (Speedup: 5.48x)

2. **Quantum ESPRESSO (MPI scaling)**:
   Detailed timing logs and parallel speedup data recorded in ``benchmark_results.json``.
   *Note*: On hybrid Intel Core processors, setting ``OMP_NUM_THREADS=1`` is critical
   to avoid OpenMP/OpenMPI thread affinity collisions.

3. **NWChem (MPI scaling)**:
   Tested on 4 MPI ranks with ZORA-B3LYP; see ``ch3_zora_b3lyp_prop.outN4``.

Files in this Directory
-----------------------
* ``benchmark_results.json``: Complete QE timing data.
* ``mopac_outputs/``: MOPAC logs for 1, 2, 4, 8, 16, and 24 threads.
* ``ch3_zora_b3lyp_prop.outN4``: NWChem 4-rank parallel execution output.
