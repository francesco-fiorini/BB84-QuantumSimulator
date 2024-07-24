# Quantum Key Distribution (QKD) BB84 Implementation with Qiskit

This software includes a Qiskit implementation of the BB84 quantum key distribution protocol in the case of a partial intercept-resend eavesdropping attack. The network scenario also incorporates channel noise, modeled with the corresponding readout error probability of the receiver backends used. The implementation explicitly calculates the Quantum Bit Error Rate (QBER) level detected between the sender and receiver and computes the estimated interception density from this. This security analysis is intended to be useful in reference to an intrusion detection system for the protocol.

## Table of Contents
- [Introduction](#introduction)
- [Installation and Usage](#installation-and-usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Quantum Key Distribution (QKD) is a method for secure communication that uses quantum mechanics to ensure the privacy of cryptographic keys. The BB84 protocol is one of the first and most well-known QKD protocols. This implementation demonstrates how QKD can be affected by an intercept-resend attack and incorporates realistic channel noise using Qiskit.

## Installation and Usage
For installation, please refer to the quantum-solver library presented by Daniel Escanez-Exposito in https://github.com/jdanielescanez/quantum-solver. The code for this implementation is intended to replace the existing BB84 folder in `src/crypto`. Therefore, it is required to replace the mentioned folder with the current package.


