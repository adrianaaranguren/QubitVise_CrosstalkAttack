# QubitVise: Double-Sided Crosstalk Attack in Superconducting Quantum Computers

QubitVise is a research project investigating security vulnerabilities in multi-tenant superconducting quantum computers. The project introduces a novel **double-sided crosstalk attack**, where malicious quantum circuits placed on both sides of a victim circuit induce interference and alter computation outcomes without direct access to the victim's qubits.

This work was accepted at the **Quantum Security (QSec) 2025 Workshop** and evaluates the attack on cloud-accessible **Rigetti Ankaa-3** quantum hardware through **Amazon Braket**.

## Overview

In cloud-based quantum computing environments, multiple users may share the same quantum processing unit (QPU). QubitVise demonstrates how an attacker can exploit CNOT-gate-induced crosstalk to influence neighboring users' computations despite logical isolation.

Key findings include:

* Introduction of a novel double-sided crosstalk attack model.
* Experimental validation on real quantum hardware.
* Evaluation using Bell State, Ising, and GHZ benchmark circuits.
* Up to **35% higher Total Variation Distance (TVD)** compared to traditional single-sided attacks.
* Average **13% increase in attack effectiveness** across tested circuits.

## Repository Contents

* `src/` – Experiment and attack implementation code
* `analysis/` – Data processing and TVD calculations
* `results/` – Experimental outputs and figures
* `presentation/` – Conference presentation slides
* `paper/` – Accepted workshop paper

## Technologies

* Python
* Amazon Braket
* qBraid
* Rigetti Ankaa-3 Quantum Computer
* Quantum Circuit Simulation and Analysis

## Research Paper

**QubitVise: Double-Sided Crosstalk Attack in Superconducting Quantum Computers**

Authors:

* Adriana Aranguren Arellano
* He Xie
* Jakub Szefer

Accepted at the Quantum Security (QSec) 2025 Workshop.

## Citation

If you use this repository in academic work, please cite the associated paper.

```bibtex
@inproceedings{aranguren2025qubitvise,
  title={QubitVise: Double-Sided Crosstalk Attack in Superconducting Quantum Computers},
  author={Aranguren Arellano, Adriana and Xie, He and Szefer, Jakub},
  year={2025}
}
```
