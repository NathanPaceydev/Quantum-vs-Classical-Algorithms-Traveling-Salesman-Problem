# Quantum-vs-Classical-Algorithms-Traveling-Salesman-Problem

## Overview

This mini-project for the University of Waterloo Institute of Quantum Computing (IQC) focuses on implementing and comparing classical algorithms with the Quantum Approximate Optimization Algorithm (QAOA) for solving the Traveling Salesman Problem (TSP). The project is showcased in two Jupyter Notebooks: `ClassicalTSP.ipynb` and `QAOATSP.ipynb`.

## Classical Approach

The classical approach to solving the TSP is presented in `ClassicalTSP.ipynb`. It involves the use and comparison of two distinct algorithms:

- **Brute Force Algorithm**: This method enumerates all possible paths and selects the shortest one. While straightforward, it's typically resource-intensive in terms of computation time.
  
- **Dynamic Programming (Held-Karp Algorithm)**: An optimized approach that leverages dynamic programming to reduce computational complexity and improve efficiency, particularly in memory usage and execution time.

Both methods are analyzed in terms of their memory usage and runtime to provide insights into their practicality for solving TSP.


## Quantum Approach

In `QAOATSP.ipynb`, we delve into the Quantum Approximate Optimization Algorithm (QAOA) as an innovative approach for addressing the TSP. This section of the project demonstrates the application of quantum computing techniques to a classical optimization problem. The notebook covers the following key aspects:

### Setting Up the Quantum Circuit
- **Initial State Preparation**: The quantum circuit begins by preparing qubits in a superposition state, allowing exploration of multiple solutions simultaneously.
- **Cost and Mixer Hamiltonians**: The TSP is encoded into a quantum format using cost Hamiltonians, which represent the problem constraints, and mixer Hamiltonians, which facilitate exploration of the solution space.

### Parameter Optimization
- **Variational Principle**: QAOA uses a variational approach, where quantum gates are parameterized by a set of angles. These parameters are tuned to minimize the cost function associated with the TSP.
- **Hybrid Optimization**: The algorithm employs a classical optimizer to adjust the parameters of the quantum circuit, seeking to find the most efficient route that minimizes the total distance.

### Quantum State Evolution
- **Layered Circuit Architecture**: The QAOA circuit comprises alternating layers of cost and mixer Hamiltonians. These layers collectively guide the quantum state toward the optimal solution.
- **Quantum Interference and Amplitude Amplification**: By exploiting quantum mechanics principles, the algorithm enhances the amplitudes of states corresponding to more optimal solutions, thereby increasing their probability of being measured.

### Performance Analysis
- **Runtime and Resource Utilization**: The efficiency of the QAOA in solving the TSP is evaluated by comparing its runtime and quantum resource utilization against classical methods.
- **Solution Quality and Probabilities**: The final quantum state is measured to obtain a probability distribution of possible solutions, with higher probabilities indicating more optimal routes.
- **Comparative Advantage**: This section assesses the potential advantages of using quantum algorithms over classical approaches for specific instances of the TSP.

### Practical Considerations
- **Scalability and Quantum Advantage**: Discussion on the scalability of the QAOA approach and the conditions under which it may offer a quantum advantage.
- **Limitations and Challenges**: Insights into the limitations of current quantum technology in solving large-scale instances of the TSP and potential future directions.

