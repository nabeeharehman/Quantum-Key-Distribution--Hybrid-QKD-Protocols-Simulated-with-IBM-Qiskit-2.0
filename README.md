# Quantum-Key-Distribution--Hybrid-QKD-Protocols-Simulated-with-IBM-Qiskit-2.0
A Qiskit-based simulator for GHZ quantum key distribution that tests real-world security using noise, eavesdropping attacks, stabilizers, and the Mermin inequality.


# 🔐 Quantum Key Distribution Security Simulator

A Python–Qiskit based framework for simulating and stress-testing multiple Quantum Key Distribution (QKD) protocols under realistic conditions such as noise, eavesdropping, and adaptive defense strategies.

This project implements and compares:

- **B92** – minimalist prepare-and-measure QKD  
- **E91** – entanglement-based Bell-test QKD  
- **GHZ-QKD** – three-party quantum key distribution with stabilizer & Mermin tests  
- **Hybrid Adaptive Protocol** – dynamically switches between protocols using a probability model when attack risk increases

---

## 🚀 Project Goals

This simulator does not only generate keys — it actively verifies quantum security.

Instead of trusting the quantum channel, the system:

- Injects depolarizing noise  
- Simulates intercept–resend eavesdropping  
- Computes QBER, stabilizers, Bell/Mermin correlators  
- Uses a risk-based hybrid model to adapt the protocol when anomalies are detected  

---

## 🔎 Implemented Security Metrics

| Metric | Description |
|------|-------------|
| QBER | Quantum Bit Error Rate for key integrity |
| XXX Stabilizer | GHZ entanglement integrity check |
| Mermin Inequality | Multipartite Bell test for GHZ states |
| Bell Violation (E91) | Detects Eve using CHSH inequality |
| Resource Efficiency | Key bits per quantum round |
| Attack Risk Score | Drives hybrid protocol switching |

---

## 🧠 Hybrid Adaptive Protocol

When the system detects increasing noise or Bell-violation degradation, it dynamically changes strategy:

| Risk Level | Active Protocol |
|-----------|----------------|
| Low Risk | GHZ-QKD |
| Medium Risk | E91 |
| High Risk | B92 |

This allows the channel to preserve security even under active attack.

---

## ⚙ Features

- Three-party entanglement using GHZ states  
- Phase-GHZ support `( |000⟩ + i|111⟩ ) / √2`  
- Configurable depolarizing noise  
- Eve intercept–resend attacks  
- Early termination on stabilizer failure  
- Modular protocol architecture  

---

## 🧩 Why This Project Matters

This framework shows that quantum security is not just about key generation , it is about preserving entanglement itself.  
The moment quantum correlations degrade, the system exposes it mathematically.

This project bridges theory, circuits, and protocol-level defense into one adaptive security engine.

---

## 🧪 Built With

- Python  
- Qiskit & Aer Simulator  
- NumPy  

---

## 📜 License

MIT License – free to use for research and education.



