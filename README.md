# Empirical Mode Decomposition

<img src="https://github.com/nebojsa55/Empirical-Mode-Decomposition/blob/master/doc/emd_gif.gif" width="600" height="400"/>

An example and introduction to EMD (Empirical mode decomposition) algorithm. EMD is the basis for [HHT](https://en.wikipedia.org/wiki/Hilbert%E2%80%93Huang_transform) and is very suitable for work with non-stationary signals.

## Definiton

Empirical Mode Decomposition is a simple iterative process that breaks the signal into components called **intrinsic mode functions (IMF)**. Every IMF contains the highest frequency of the signal in the previous iteration, thus enabling high-frequency noise rejection.  

IMF is defined as the function that satisfies the following two requirements:

1. The number of extrema and the number of zero-crossings in the dataset must either be **equal** or **differ at most by one**
2. The mean value of the envelope defined by the local maxima and the envelope defined by the local minima is zero.

## Other Python packages

This script will show the implementation of classical EMD algorithm. For other kinds of EMD, such as ensemble EMD, please refer to:

![PyPI](https://img.shields.io/pypi/v/emd?color=red&label=emd)

### Installation

To install emd package, insert the command:
```shell
> pip install emd
```
