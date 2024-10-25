# QOSF-Screening-Task
Added Task 1 and 2
## Quantum Circuit Simulation Tasks
This project contains implementations and analyses of various quantum simulation techniques, providing foundational insights into how quantum computations are performed in a classical environment. \\

### Task 1: Statevector Simulation of Quantum Circuits
** 1. Naive Simulation Using Matrix Multiplication **
Goal: Simulate an n-qubit quantum circuit by representing quantum states and gates as matrices. \\
Method: Utilized matrix multiplication (using Kronecker products) to sequentially apply gates (X, H, CNOT) on initial state vectors. \\
Performance: Ran simulations for increasing qubit numbers, plotting runtime versus qubit count to evaluate scalability limits. \\
** 2. Advanced Simulation Using Tensor Multiplication **
Goal: Optimize statevector simulation by representing states as n-dimensional tensors, making operations more efficient. \\
Method: Replaced matrix multiplication with tensor contraction (using np.tensordot or np.einsum) for applying gates directly to specific qubit axes. \\
Performance: Compared runtime to the naive method, providing a runtime plot and discussing performance improvements with this approach. \\
** 3. Bonus: Final State Sampling **
Objective: Introduced methods to simulate measurement by sampling from the resulting statevector or tensor representation. \\
Approach: Discussed potential sampling techniques and their implications for interpreting quantum measurement outcomes. \\

