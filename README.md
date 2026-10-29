# quantum-lhc-anomaly-detector
# ⚛️ Quantum Anomaly Detector for LHC Particle Collisions
An experimental quantum machine learning project that applies **Quantum Support Vector Classifiers (QSVC)** to detect rare, exotic particle physics anomalies (such as dark matter candidates or supersymmetric signatures) hidden within high-background Standard Model LHC collision data.

---

## 🔬 Physics & Quantum Computing Framework

At the Large Hadron Collider (LHC), isolating rare physics signals from massive QCD backgrounds is a major big-data challenge. This project explores **Quantum Machine Learning (QML)** by mapping classical particle collision kinematics into high-dimensional quantum Hilbert spaces.

### 1. Feature Encoding via Quantum Circuits
Collision features—such as transverse momentum ($p_T$) and pseudorapidity ($\eta$)—are encoded into qubit quantum states ($|\psi(x)\rangle$) using an entangled **$ZZFeatureMap$** circuit:
$$U_{\phi(x)} = \exp\left(i \sum_{i,j} \phi(x_i)\phi(x_j) Z_i Z_j\right)$$

### 2. Quantum Kernel Estimation
A quantum kernel matrix $K_{ij} = |\langle \psi(x_i) | \psi(x_j) \rangle|^2$ is computed by measuring statevector fidelity on quantum simulators, capturing complex non-linear correlations that classical kernels might miss.

---

## ✨ Key Features

* **Synthetic LHC Dataset Generator:** Simulates Standard Model background vs. exotic high-$p_T$ anomaly collision distributions.
* **Qiskit Quantum Kernel Pipeline:** Integrates `ZZFeatureMap` and `FidelityQuantumKernel` with Scikit-Learn's Support Vector Classifier.
* **Decision Boundary Visualization:** Generates classification boundary plots separating background noise from quantum-classified signals.

---

## 🛠️ Tech Stack

* **Quantum SDK:** Qiskit, Qiskit Machine Learning
* **Machine Learning:** Scikit-Learn, NumPy
* **Visualization:** Matplotlib
* **Environment:** Google Colab / Jupyter Notebooks


Result (https://github.com/Vruti-Soni/quantum-lhc-anomaly-detector/blob/main/Vector%20classifier.png)
