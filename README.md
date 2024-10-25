# QOSF-Screening-Task
Added Task 1 and 2
## Quantum Circuit Simulation Tasks
This project contains implementations and analyses of various quantum simulation techniques, providing foundational insights into how quantum computations are performed in a classical environment. 

### Task 1: Statevector Simulation of Quantum Circuits

** 1. Naive Simulation Using Matrix Multiplication **

Goal: Simulate an n-qubit quantum circuit by representing quantum states and gates as matrices. 

Method: Utilized matrix multiplication (using Kronecker products) to sequentially apply gates (X, H, CNOT) on initial state vectors. 

Performance: Ran simulations for increasing qubit numbers, plotting runtime versus qubit count to evaluate scalability limits. 

** 2. Advanced Simulation Using Tensor Multiplication **

Goal: Optimize statevector simulation by representing states as n-dimensional tensors, making operations more efficient. 

Method: Replaced matrix multiplication with tensor contraction (using np.tensordot or np.einsum) for applying gates directly to specific qubit axes. 

Performance: Compared runtime to the naive method, providing a runtime plot and discussing performance improvements with this approach. 

** 3. Bonus: Final State Sampling **

Objective: Introduced methods to simulate measurement by sampling from the resulting statevector or tensor representation. 

Approach: Discussed potential sampling techniques and their implications for interpreting quantum measurement outcomes. 

## Task 2: Noise, Noise, and More Noise

This task addresses noise challenges in quantum computing, building functions to simulate noise, optimize gate basis, perform quantum addition, and analyze noise effects.

### 1. Noise Model

Objective: Add Pauli noise after each gate. 

Approach: Created a function to inject random Pauli operators (X, Y, Z) based on probability parameters α (for one-qubit gates) and β (for two-qubit gates).

### 2. Gate Basis Transformation

Objective: Transform a quantum circuit into a limited gate set {CX, ID, RZ, SX, X}.

Approach: Constructed a function to rewrite circuits to this gate set, supporting standard quantum hardware.

### 3. Quantum Addition with Draper Adder

Objective: Implement quantum addition using the Draper adder algorithm.

Approach: Constructed the Quantum Fourier Transform (QFT) from scratch, facilitating number addition on quantum circuits.

### 4. Analyzing Noise Effects

Objective: Study noise impact on the quantum addition circuit.

Approach: Ran simulations across noise levels to evaluate noise effects on addition accuracy, exploring strategies to mitigate noise and the influence of gate count.

Each section includes annotated code, runtime analysis, and insights for handling noise in quantum operations.
