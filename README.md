# CasADi-Based Lap Time Simulation

This project uses **CasADi**, **NumPy**, **SciPy**, and **Matplotlib** for symbolic modeling and optimization, and runs in **Jupyter Notebook** for interactive visualization.

---

## Dependencies

| Package     | Version    |
|-------------|------------|
| Python      | 3.13.5     |
| NumPy       | 2.1.3      |
| SciPy       | 1.15.3     |
| Matplotlib  | 3.10.0     |
| Jupyter     | latest     |
| CasADi      | 3.7.0 (compiled manually) |

---

## Step-by-Step Setup

### 1 Create the Conda Environment (Without CasADi Yet)

```bash
conda create -n casadi_py313_env python=3.13.5 -y
conda activate casadi_py313_env
```
---

### 2 Install Required Packages (except CasADi)

```bash
conda install -y numpy=2.1.3 scipy=1.15.3 matplotlib=3.10.0 jupyter cmake swig
```
---

### 3 Install CasADi Using pip

```bash
pip install casadi==3.7.0
```
---
## 4 Running Jupyter Notebook

```bash
jupyter notebook
```
Open the ```LapTime_Sim.ipynb``` notebook file and start working.

---
## 5 File Structure

```
.
├── LapTime_Sim.ipynb      # Main notebook file
├── README.md                   # This file
└── Trackdata20.mat             # Test Track Data from DRe20
```

##  6 Verify Installation
Run the following Python code to check versions:
```
import casadi
import numpy as np
import matplotlib
import scipy

print("CasADi version:", casadi.__version__)
print("NumPy version:", np.__version__)
print("Matplotlib version:", matplotlib.__version__)
print("SciPy version:", scipy.__version__)
```