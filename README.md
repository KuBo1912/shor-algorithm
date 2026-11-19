# Quantum Order-Finding & Shor's Algorithm

End-to-end implementation of **Quantum Order-Finding** and **Shor's Factoring Algorithm** using Qiskit & NumPy, following Chapter 5 of *Quantum Computation and Quantum Information* (Nielsen & Chuang).

## Contents
- `build_find_order.ipynb`: Quantum Order-Finding pipeline for arbitrary $N$ and coprime $x$:
  1. Custom `build_inverse_qft` and `build_qpe` (reused from `qpe_benchmark`).
  2. Generalized modular multiplication oracle $U_x\vert y\rangle = \vert xy \bmod N\rangle$ via $2^L \times 2^L$ permutation `UnitaryGate`.
  3. Phase estimation & sampling on `AerSimulator`.
  4. Classical Continued Fractions post-processing to extract order $r$.
