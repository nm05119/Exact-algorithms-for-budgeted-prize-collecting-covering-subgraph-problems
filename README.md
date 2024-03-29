---------------------------------------------------------------------------------------------------------------
authors: Nicola Morandi, Roel Leus, Hande Yaman

affiliation: ORSTAT group, Faculty of Economics and Business, KU Leuven, Belgium

Exact algorithms for budgeted prize-collecting covering subgraph problems
---------------------------------------------------------------------------------------------------------------

This public repository contains the instances, the parameter settings and the computational results
of the two cases of budgeted prize-collecting covering subgraph problems considered in the paper mentioned above.

For the definition of the symbols and the terms hereby used, and for references to the original sources of the 
instances, we refer to the paper mentioned above.

The directory "Instances" contains seven .inst files, corresponding to the six base instances considered in the paper,
and to the instance shown in Figure 1 of the paper. The first line of these files contains the number of vertices of
the instance. All the other lines, one for each vertex v, contains in the order: the x-coordinate, the y-coordinate
and the full prize p_v, separated by a space. All the base instances are Euclidean and symmetric.

Each of the two directories "Cycle-BPCCSP" and "Tree-BPCCSP" contain the following three subdirectories: "Parameters",
"Branch-and-Cut" and "Benders". The subdirectories "Parameters" contain six .param files. The .param files contain 72
lines each, and each line corresponds to a generated instance. Every such line contains in the order, and separated
by a space: the value for L, the value for r_v for every vertex v, the value for c_v for every v, the value of the ratio
q_vw / p_v, and the boolean 1 if it is the first line or 0 otherwise (for scripting purposes).

Both the "Branch-and-cut" and "Benders" subdirectories contain six .out files. Each line of an .out file contains the
computational results corresponding to a single instance. The definition of the values contained in each .out file is
in its first line. If an instance was not solved within the time limit, i.e., 3600 seconds, then the final MIP gap is given
between parenthesis instead of the optimal value. If an instance could not be solved because of the solver running out
of memory, then the corresponding line was removed from the .out file.

----------------------------------------------------------------------------------------------------------------

Morandi, N., Leus, R., & Yaman, H. (2022). Exact algorithms for budgeted prize-collecting covering subgraph problems.
Computers & Operations Research, volume 144, 105798.
