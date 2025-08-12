TITLE:
Replication data for: HDNNP for Co3O4

AUTHORS:
Amir Omranpour, Lehrstuhl für Theoretische Chemie II, Fakultät für Chemie und Biochemie, Ruhr-Universität Bochum

Jörg Behler, Lehrstuhl für Theoretische Chemie II, Fakultät für Chemie und Biochemie, Ruhr-Universität Bochum


CONTACT:
Amir.Omranpour@ruhr-uni-bochum.de


CITATION:
Omranpour, Amir; Behler, Jörg, 2024, "Replication Data for: HDNNP for Co3O4", https://doi.org/10.17877/RESOLV-2024-m3rb0526, TUDOdata, V1"


RELATED CITATION:
A. Omranpour and J. Behler, “A High-Dimensional Neural Network Potential for Co3O4”, https://arxiv.org/abs/2409.11037, 2024. 


PROJECT DESCRIPTION:
The data files contain the raw input files for training the neural network, the required input files with the settings for the RuNNer code, and the resulting weights and scaling data used to perform the MD simulations reported in the paper.


Date of creation: 27th November 2024 
File format: txt 
List of files: 
- input.data
- input.nn
- opt.weights.008.out
- opt.weights.027.out
- scaling.data

DATASET DESCRIPTION:
Important Note: The format of all files (including the unit used) are according to the RuNNer package version 1.3, and for detailed explanations of each file and keyword, please refer to the RuNNer documentation website: https://theochemgoettingen.gitlab.io/RuNNer/1.3/

- input.data: (see the RuNNer documentation) The input.data file contains all the reference structures. Each structure in the input.data file is framed by a pair of a begin and an end keyword. It includes all the structures used for training/testing the neural network. in a single input.data file. The order of the lines in between begin and end is arbitrary and each line is free-formatted. For each atom in the system there is one line starting with the keyword atom, followed by three numbers specifying the Cartesian coordinates (in Bohr). Then the element symbol is given, followed by a number for the atomic charge, followed by atomic forces Fx, Fy and Fz. For each structure, there is a keyword named "energy" which is the total energy of the system. The unit for length is Bohr and the unit for is Hartree, and the unit for force is Hartree/Bohr.
- input.nn: (see the RuNNer documentation) The input.nn file is the main control file of RuNNer. The keywords can be given in arbitrary order, and blank lines and commented lines (starting with #) are permitted. If keywords are not specified, reasonable defaults are assumed where possible and written to the output for information. All the keywords used in this file are documented in the reference section of RuNNer documentation.
- opt.weights.008.out: (see the RuNNer documentation) The weights for the Atomic Neural Network for Oxygen (i.e. element 8).
- opt.weights.027.out: (see the RuNNer documentation) The weights for the Atomic Neural Network for Cobalt (i.e. element 27).
- scaling.data:(see the RuNNer documentation) This file is written during the fitting process. It contains the minimum, maximum and average value for each symmetry function for the short range NN. It is a mandatory input file for the prediction of energies for new structures. In runner_mode 2 a scaling.data file can be read using the keyword use_old_scaling. This can be required to keep exactly the same fit (the file scaling.data is part of the fit) when restarting runner_mode 2 with a modified training set.

