---------------------------------------------------------------------------------------------------------------
Exact methods for budgeted prize-collecting covering subgraph problems

authors: Nicola Morandi, Roel Leus, Hande Yaman
affiliation: ORSTAT group, Faculty of Economics and Business, KU Leuven, Belgium
---------------------------------------------------------------------------------------------------------------

This public repository contains the instances, the parameter settings and the computational results
of the two cases of budgeted prize-collecting covering subgraph problems considered in the paper mentioned above.

For the definition of the symbols and the terms here used, we refer to the paper mentioned above.

The directory "Instances" contains six .inst files, corresponding to the six base instances considered in the paper.
The first line contains the number of vertices of the instance. All the other lines, one for each vertex v, contains
in the order: the x-coordinate, the y-coordinate and the full prize p_v, separated by a space. All the base instances
are Euclidean and symmetric.

Each of the two directories "Tour-BPCCSP" and "Tree-BPCCSP" contain the following three subdirectories: "Parameters",
"Branch-and-Cut" and "Benders". The subdirectories "Parameters" contain six .param files. The .param files contain 72
lines each, and each line corresponds to a generated instance. Every such line contains in the order and separated
by a space: the value for L, the value for r_v for every vertex v, the value for c_v for every v, the value of the ratio
q_vw / p_v and 1 if it is the first line or 0 otherwise (for scripting purposes).

Both the "Branch-and-cut" and "Benders" subdirectories contain six .out files. Each line of an .out file contains the
computational results on a single instance. Several computationally-relevant values are given about every instance,
according to the first line of the .out files. If an instance was not solved within the time limit, i.e., 3600 seconds,
then the final gap is given between parenthesis instead of the optimal value. If an instance could not be solved because
of the solver running out of memory, all the values in the corresponding line are replaced with "-".
