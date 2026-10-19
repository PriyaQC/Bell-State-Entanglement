# Bell-State-Entanglement
A beginner quantum computing project simulating Bell-State entanglement using NumPy and Qiskit.
# Quantum Simulation of Superposition and Entanglement: A NumPy–Qiskit Study

## Overview

This project explores the preparation and simulation of a two-qubit Bell state using Python, NumPy, and Qiskit. It connects basic linear algebra with quantum circuits, measurement probabilities, and a mathematical test for entanglement.

This is an educational project developed while learning the foundations of quantum computing.

## Objectives

* Construct a Bell state using matrix operations in NumPy.
* Prepare the same state using Hadamard and CNOT gates in Qiskit.
* Compare theoretical probabilities with simulated measurement results.
* Visualize measurement counts using Matplotlib.
* Examine entanglement using the coefficient-matrix determinant test for pure two-qubit states.

## Mathematical Background

The Bell state studied in this project is

$$
|\Phi^+\rangle=\frac{|00\rangle+|11\rangle}{\sqrt{2}}.
$$

It is prepared by applying a Hadamard gate to the first qubit, followed by a CNOT gate with the first qubit as the control and the second as the target.

For an ideal circuit, the theoretical measurement probabilities are:

| Outcome | Probability |
| ------- | ----------: |
| 00      |         0.5 |
| 01      |           0 |
| 10      |           0 |
| 11      |         0.5 |

## Tools and Technologies

* Python
* NumPy
* Qiskit
* Qiskit Aer
* Matplotlib
* Google Colab

## Project Workflow

1. Define the computational basis and quantum gates using NumPy.
2. Construct the Bell state through matrix operations.
3. Build the equivalent quantum circuit in Qiskit.
4. Compare the state probabilities from both approaches.
5. Simulate repeated measurements and visualize the counts.
6. Apply the determinant test to examine pure-state entanglement.

## Results

The ideal Bell-state simulation predicts nonzero probabilities only for outcomes `00` and `11`, each with probability 0.5. The NumPy and Qiskit probability calculations are expected to agree.

Finite-shot measurement counts may differ slightly from a perfect 50:50 split because of sampling variation.

The final numerical results and measurement graph are available in the project notebook.

## Limitations

This project uses an ideal quantum simulator and does not demonstrate execution on physical quantum hardware. The determinant test described here applies to pure two-qubit states; it is not a general entanglement test for mixed states.

## How to Run

1. Open `BELL_STATE_ENTANGLEMENT.ipynb`.
2. Open the notebook in Google Colab.
3. Run the cells in order.
4. Install the required packages if prompted by the notebook.

## Future Learning

Possible extensions include studying other Bell states, exploring quantum noise, and comparing ideal simulations with noisy circuits.

## Author

An Applied Mathematics undergraduate learning Python, linear algebra, and quantum computing and quantum mechanics.

This repository documents my learning and implementation process; it is not presented as original research.
