# Intel Quantum Simulator

The Intel Quantum Simulator, also known as qHiPSTER (The Quantum High Performance Software Testing Environment),
is a simulator of quantum circuits coded to take maximum advantage of multi-core and multi-nodes architectures.
It is based on a complete representation of the qubit register state in terms of a distributed vector, while
operations and gates are never explicitely represented in terms of matrices.
qHiPSTER uses MPI (message-passing-interface) protocols to store and manipulate the quantum state for 
both intra- and inter-node operations.


## Installation

Intel Quantum Simulator builds as a static library. After cloning the repository, compile it via:

```bash
  git clone https://github.com/intel/Intel-QS.git
  cd Intel-QS
  make all
```

The default building process requires [Intel Math Kernel Library](https://software.intel.com/en-us/mkl)
and the [MPI-ICPC compiler](https://software.intel.com/en-us/node/528770).
These choices can be personalized by editing (for example with [VIM](http://www.vim.org/>)) the file:

```bash
  vim make.inc
```

Documentation is automatically generated by running:

```bash
  make docs-clean
  make docs-doxy
```

## Getting started

The simplest way of familiarize with qHiPSTER is by exploring the examples provided in the ```tests/``` folder.
In particular, the code ```tests/getting_started_example.cpp``` provides step-by-step description of the main commands:
define a qubit register object, perform quantum gates, measure one or multiple qubits.


## How to contribute

Thanks for your interest in the project! We welcome pull requests from developers of all skill levels.

If you find a bug or want to propose a new feature, open an issue.
If you have written some code that should be merged, open a pull request describing your changes and why it should be merged.
If you have a question or want to discuss something, feel free to send an email to [Justin Hogaboam](justin.w.hogaboam@intel.com)
or [Gian Giacomo Guerreschi](gian.giacomo.guerreschi@intel.com).


## How to cite

When using the Intel Quantum Simulator for research projects, please cite:

    Mikhail Smelyanskiy, Nicolas P. D. Sawaya, Alán Aspuru-Guzik
    *qHiPSTER: The Quantum High Performance Software Testing Environment*
    [arXiv:1601.07195](https://arxiv.org/abs/1601.07195)__\(2016\).

