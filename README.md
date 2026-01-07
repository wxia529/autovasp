# VASP HDF5-Enabled Workflow

This repository provides a reproducible computational workflow for **VASP (Vienna Ab initio Simulation Package)** compiled with **HDF5 support**, enabling efficient I/O for large-scale DFT calculations via the `vaspout.h5` file.

## Features

- Automated setup and execution of VASP jobs with HDF5 output.
- Tools to parse and analyze `vaspout.h5` using and `py4vasp`.
- Integration-ready structure for high-throughput or machine learning workflows.
- Compatibility with VASP ≥6.3 (HDF5 support officially introduced in 6.3.0).

## Prerequisites

- **VASP** compiled with HDF5 support (`-Dusehdf5` flag in `makefile.include`).
  - Ensure `libhdf5` and development headers are installed on your system.
- Python ≥3.8 with the following packages:
  ```bash
  pip install h5py py4vasp numpy ase pymatgen
  ```
- A valid `POTCAR` library and `INCAR`/`KPOINTS` templates for your system.

## Workflow Overview
