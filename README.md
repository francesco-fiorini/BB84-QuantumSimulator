# Quantum Key Distribution (QKD) BB84 Implementation with Qiskit

This software includes a Qiskit implementation of the BB84 quantum key distribution protocol in the scenario of a partial intercept-resend eavesdropping attack. The network scenario also incorporates channel noise, modeled with the corresponding readout error probability of the receiver backends used. The implementation explicitly calculates the Quantum Bit Error Rate (QBER) level detected between the sender and receiver and computes the estimated interception density from this. This security analysis is intended to be useful in reference to an intrusion detection system for the protocol.

## Table of Contents
- [Introduction](#introduction)
- [Installation and Usage](#installation-and-usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Quantum Key Distribution (QKD) is a method for secure communication that uses quantum mechanics to ensure the privacy of cryptographic keys. The BB84 protocol is one of the first and most well-known QKD protocols. This implementation demonstrates how QKD can be affected by an intercept-resend attack and incorporates realistic channel noise using Qiskit.

## Installation and Usage
For installation, refer to the Quantum-Solver library presented here. The code for this implementation is intended to replace the existing BB84 folder in `src/crypto`. Therefore, it is required to replace the mentioned folder with the current package.

Example usage:
```python
from bb84_simulation import BB84Simulation

# Initialize the simulation
simulation = BB84Simulation(num_qubits=100, intercept_prob=0.1, readout_error_prob=0.02)

# Run the simulation
qber, interception_density = simulation.run()

# Output the results
print(f"QBER: {qber}")
print(f"Interception Density: {interception_density}")
