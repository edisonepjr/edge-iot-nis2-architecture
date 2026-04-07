# Resilient Edge-IoT Architecture for Environmental Monitoring in Critical Infrastructure (NIS2-Hardened)

## 📌 Overview

This project presents a low-cost, resilient Edge-IoT architecture designed for environmental monitoring in critical infrastructure scenarios. The solution integrates cybersecurity principles aligned with the NIS2 Directive, focusing on local processing, fault tolerance, and secure data handling.

The architecture avoids full cloud dependency by implementing edge-based resilience mechanisms, ensuring continued operation under network disruption scenarios.

---

## 🎯 Objectives

- Provide a **low-cost alternative** to industrial monitoring systems (e.g., PLC-based solutions)
- Implement **resilient data collection** using Edge computing
- Apply **cybersecurity best practices** aligned with:
  - NIS2 Directive
  - IEC 62443
  - NIST Cybersecurity Framework (CSF)

---

## 🏗️ Architecture

The system is based on a distributed cluster of ESP32 nodes connected to sensors, performing local data processing and secure transmission.

### Key Components:

- ESP32 microcontrollers (sensor nodes)
- Edge processing layer (cluster-based logic)
- Secure communication module
- Local storage (SD card)
- Optional cloud integration (non-critical)

### Design Principles:

- **Store-and-forward mechanism**
- **Decentralized resilience**
- **Secure-by-design approach**

---

## 🔐 Security Features

- AES-256-GCM encryption for data in transit
- Secure Boot enabled on ESP32
- Disabled debug interfaces (JTAG/UART)
- Authentication and integrity validation
- Local fallback operation (offline mode)

---

## ⚙️ Technologies Used

- ESP32 (primary hardware platform)
- Embedded C / Arduino framework
- AES-256-GCM cryptography
- SD card storage module
- Wireless communication (Wi-Fi)

---

## 📊 Key Contributions

- Demonstrates a **cost-effective alternative** to traditional industrial monitoring systems
- Implements **resilience without full cloud reliance**
- Integrates **regulatory-aligned security (NIS2-inspired design)**
- Provides a **practical architecture for critical infrastructure scenarios**

---

## ⚠️ Limitations

- Prototype-level implementation (not industrial-grade certified)
- Limited large-scale deployment validation
- Security model based on best practices, not formal certification

---

## 📄 Publication

This project is based on the following academic work:

**"Arquitetura Edge-IoT Resiliente e NIS2-Hardened para Monitoramento Ambiental em Infraestruturas Críticas"**  
Revista Eletrônica de Iniciação Científica em Computação (REIC)  
Status: Accepted for publication (2026)

---

## 🔗 Future Work

- Integration with real-time anomaly detection (AI-based)
- Expansion to larger distributed clusters
- Formal compliance validation against NIS2 and IEC 62443
- Performance benchmarking under real-world conditions

---

## 👨‍💻 Author

Edison Pereira Junior  
Computer Engineering Student  
Brazil

---

## 📜 License

This project is provided for academic and research purposes.
