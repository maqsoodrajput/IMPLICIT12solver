# IMPLICIT12solver - A Fast Atmospheric Chemistry Solver

This solver gives a 5X speed-up for the ICON-ART climate model. It can also be used in any climate model that uses the KineticPreProcessor KPP (https://github.com/KineticPreProcessor/KPP).

This solver is inspired by the IMEX solver. However, an explicit solver is not possible in the case of stiff atmospheric chemistry problems.
This solver consists of:
- Backward Euler: L-stable, 1 stage, order 1 with the Fixed step size
- Adaptive Sdirk 2a: L-stable, 2 stages, order 2 with automatic step size selection 

 

### Usage
This repository only contains two files. Please copy both files, "implicit12.f90" and "implicit12.def," to the directory "kpp/int/."
This can also be used with the CAABA/MECCA box model (https://gitlab.com/RolfSander/caaba-mecca).
