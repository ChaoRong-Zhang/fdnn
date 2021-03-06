# Description

The Python code in this repository implements the neural network based non-linear self-interference cancellation method desribed in [1], as well as a baseline polynomial non-linear self-interference canellation method for comparison purposes. The ZIP file also contains the measurements from a full-duplex testbed that are used as a dataset. A working installation of Keras is required to run the code. The default values in the code exactly reproduce (up to the randomness of the mini-batch learning procedure for the neural network) the results in [1].

# Contents

This python code is split into three files:

1. _NNCancellation.py_: This file loads the measured testbed data and performs non-linear cancellation using the neural network based method proposed in [1]. It also plots the PSDs of the resulting signals as well as the cancellation performance.
2. _polynomialCancellation.py_: This file loads the measured testbed data and performs non-linear cancellation using the baseline polynomial model. It also plots the PSDs of the resulting signals as well as the cancellation performance.
3. _fullduplex.py_: This file contains all the helper functions that are required to do linear cancellation and non-linear cancellation using the baseline polynomial model and it is imported in both NNCancellation.py and polynomialCancellation.py.

[1] A. Balatsoukas-Stimming, "Non-linear digital self-interference cancellation for in-band full-duplex radios using neural networks," in IEEE International Workshop on Signal Processing Advances in Wireless Communications (SPAWC), Jun. 2018
