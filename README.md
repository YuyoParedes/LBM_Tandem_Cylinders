
## Contents

This LBM code includes:

- D2Q9 lattice
- TRT collision operator
- Zou-He on all boundary conditions
- Drag/lift computation using interpolated bounce-back
- Core routines are deferred to Numba

## Running simulations

Flow simulation around cylinders in tandem arrangement is described in the `lbm/src/app/turek` repository. To run a simulation, adjust the parameters in the python file, then run `python3 start.py turek`. 
A results folder will be generated in `./results/` with the current date and time. If you wish to add a new application, you must create a new app, and register it in the factory, located in `lbm/src/app/app.py`. The computational times are obtained on a standard laptop.


