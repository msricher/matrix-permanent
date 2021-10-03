# Purpose
Efficiently evaluate the [permanent of a (rectangular) matrix](https://en.wikipedia.org/wiki/Permanent_(mathematics)). The idea is to switch between the brute-force combinatoric algorithm (more efficient for small matrices) and the more complicated [Ryser and Glynn algorithms](https://en.wikipedia.org/wiki/Computing_the_permanent) (preferable for larger matrices) based on the dimensionality of the problem. Special structure (e.g., that the matrix entries are binary, the matrix is sparse) is neither required nor exploited.

# Motivation
Many of the overlap formulas used in the Flexible Ansatz for N-electron Configuration Interaction approach rely upon evaluation of (usually small, but not always) permanents.

# Possible extensions
Evaluating the derivative of a permanent with respect to a parameter is a stretch goal.

# Notes
[Michael's notes](docs/main.pdf?raw=true)
[Example Python code (combinatoric and Glynn algorithms)](example.py)
[David's Ryser code](https://github.com/QuantumElephant/fanpy/blob/master/wfns/backend/math_tools.py)
