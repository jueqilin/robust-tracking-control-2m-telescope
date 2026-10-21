# robust-tracking-control-2m-telescope
Observer-based robust tracking control for 2m-class optical telescope 

This repository implements an **observer-based robust tracking control** 
algorithm for 2m-class optical telescopes. 
The framework handles system uncertainties, external disturbances, 
and measurement noise while ensuring high-precision tracking performance.

## Prerequisites

Before running the code, ensure your environment meets the following requirements:

- **MATLAB Version**: R2023a or later
- **Required Toolboxes**:
  - Control System Toolbox
  - Simulink 
  - [YALMIP Toolbox](https://yalmip.github.io/) 
  - [MOSEK Solver](https://www.mosek.com/) 
- **MATLAB Live Editor** (required for `.mlx` files)

## Project Structure

```
robust-tracking-control-2m-telescope/
│
├── data/                                   # Input data files
├── figures1/                               # Output figures from Simulation 1
├── figures2/                               # Output figures from Simulation 1
├── main.mlx                                # Data pre-processing and main entry point
├── analysis1.mlx                           # Data analysis for Simulation 1
├── analysis2.mlx                           # Data analysis for Simulation 2
├── ControlSystemSimulation.slx             # Core simulation model
└── Robusttrackingcontrol2mtelescope.prj    # MATLAB Project file
```


## How to run

Follow these steps **in the exact order** to reproduce the results:

### Step 1: Open the MATLAB project
**File**: `Robusttrackingcontrol2mtelescope.prj`  

Double-click this file to open the MATLAB Project. This automatically:
- Sets the correct working directory
- Adds all necessary folders to the MATLAB path
- Automatically executes `main.mlx` for data pre-processing
 
By default, `main.mlx` solves for parameters based on Simulation 1.
If you need to change the simulation mode, 
**modify `MODE` before opening the project or then re-run `main.mlx`** 

### Step 2: Open and run Simulink model
**File**: `ControlSystemSimulation.slx`

After the project opens and `main.mlx` finishes preprocessing:
  
### Step 3: Analysis output data
**File**:`analysis1` (for Simulation 1) or `analysis2` (for Simulation 2)

Depending on the mode selected in Step 2, run the corresponding analysis script

**Output**: Figures saved to `/figures1/` or `/figures2/` respectively

---

## Usage Policy

The code and data provided in this repository are for reference only. 
Any use of the code or data requires prior permission from the author. 
Please contact the author to obtain access.

Email: jueqilin@seu.edu.cn
