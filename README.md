# Quantum Key Distribution (QKD) BB84 under partial-intercept attack Qiskit Implementation

This software includes a Qiskit implementation of the BB84 quantum key distribution protocol in the case of a partial intercept-resend eavesdropping attack. The network scenario also incorporates channel noise, modeled with the corresponding readout error probability of the receiver backends used. The implementation explicitly calculates the Quantum Bit Error Rate (QBER) level detected between the sender and receiver and computes the estimated interception density from this. For this purpose, a new Excel file is created and updated with the calculated performance parameters. 
This security analysis is intended to be useful in reference to an intrusion detection system for the protocol.

## Table of Contents
- [Introduction](#introduction)
- [Installation and Usage](#installation-and-usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Quantum Key Distribution (QKD) is a method for secure communication that uses quantum mechanics to ensure the privacy of cryptographic keys. The BB84 protocol is one of the first and most well-known QKD protocols. This implementation demonstrates how QKD can be affected by an intercept-resend attack and incorporates realistic channel noise using Qiskit.

## Installation and Usage
For installation, please refer to the quantum-solver library presented by Daniel Escanez-Exposito in https://github.com/jdanielescanez/quantum-solver. The code for this implementation is intended to replace the existing BB84 folder in `quantum-solver/src/crypto`. Therefore, it is required to replace the mentioned folder with the current package.

## Features
- Implementation of the BB84 QKD protocol
- Simulation of partial intercept-resend eavesdropping attacks
- Incorporation of channel noise using readout error probabilities
- Calculation of Quantum Bit Error Rate (QBER)
- Estimation of interception density

## Contributing
Contributions are welcome! Please contact francesco.fiorini@phd.unipi.it for suggested changes.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


