# 2021-IQW
Source code for paper [A Complete Quantum Circuit to Solve the Information Set
Decoding Problem](#Authors and citations ) submitted at 2021 IEEE Quantum Week
Conference. The bibtex is available at the end of the Readme.

This repository is taken from the code available at
[https://github.com/tigerjack/qat-utils](https://github.com/tigerjack/qat-utils)
and can be run on either the open-source [myQLM
simulator](https://github.com/myQLM) or the [QLM
simulator](https://atos.net/en/solutions/quantum-learning-machine), both
provided by Atos.

# Installation #
If you would like to test the code, you can [install
myQLM](https://myqlm.github.io/myqlm_specific/install.html). 


# Tests #
The tests can be run using `python -m unittest` (all tests) or `python -m
unittest test.module_name` (only a specific test case, replacing module name
with the actual name of the module). For example, if you want to run all the
tests related to the RREF circuit, you can run `python -m unittest
test.test_qroutine_rref`.


When launching tests, you can provide some optional environment variables
  * `LOG_LEVEL`, with values equal to the names provided by Python logging
utilities. E.g. `LOG_LEVEL=DEBUG python -m unittest test.test_qroutine_rref`.
  * `SLOW_TEST_ON=1` to enable also time consuming tests 
  * `QLM_ON=1` to use the QLM instead of myQLM
  * `SIMULATOR`, to pass the name of a simulator. For myQLM, only the `pylinalg`
    simulator is actually available. For QLM, there are a variety of available
    simulators depending on the version.


# Contribution Guidelines #
If you would like to contribute to the code, please open a [GitHub
issue](https://github.com/tigerjack/qat-utils/issues) on the original [qat-utils
repository](https://github.com/tigerjack/qat-utils). This repository will be
made read-only after the conference and it is here just for reference.

# Authors and citations #
The code here was used in the results of the following articles

Simone Perriello, Alessandro Barenghi and Gerardo Pelosi,
A Complete Quantum Circuit to Solve the Information Set Decoding Problem.
In Proc. of the IEEE International Conference on Quantum Computing and Engineering,
(QCE) 2021, Broomfield, CO, USA, October 18-22, 2021 (Fully virtual event).
IEEE Computer Society 2021.
[Accepted on July 31th, 2021]
 [bibtex](/bibtex.bib)
