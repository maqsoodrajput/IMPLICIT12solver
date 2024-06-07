# IMPLICIT12solver - A Fast Atmospheric Chemistry Solver

This solver gives 5X speed-up for ICON-ART climate model. This solver can be used in any climate model which uses KPP (https://github.com/KineticPreProcessor/KPP).

This solver is inspired by IMEX solver. However, in the case of stiff atmospheric chemistry problems it is not possible to use an explicit solver.
This solver consists of:
- Backward Euler: L-stable, 1 stage, order 1 with the Fixed step size
- Adaptive Sdirk 2a: L-stable, 2 stage, order 2 with automatic step size slection 

 

### Usage
This repository only contain two files the solver file and the header file. Please copy both files "implicit12.f90" and "implicit12.def" in the directory "kpp/int/".
This can also be used with the CAABA/MECCA box model (https://gitlab.com/RolfSander/caaba-mecca).
