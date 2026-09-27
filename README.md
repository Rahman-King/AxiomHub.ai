<div align="center">

# AXION 🛡️
### *Outsmart threats before they come in sight.*

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=flat-square&logo=python)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100%2B-teal?style=flat-square&logo=fastapi)](https://fastapi.tiangolo.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3.0-cyan?style=flat-square&logo=tailwind-css)](https://tailwindcss.com/)
[![Raspberry Pi](https://img.shields.io/badge/Hardware-Raspberry_Pi_5-red?style=flat-square&logo=raspberrypi)](https://www.raspberrypi.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

</div>

---

## 🚀 Overview

**Axion** is a unified, multi-layered cybersecurity platform built to tackle modern digital threats across three distinct vectors: consumer browsing, enterprise penetration testing, and physical network hardware monitoring. By combining local heuristic AI, automated VAPT pipelines, and inline hardware-level packet sniffing, Axion provides seamless, proactive protection.

---

## 🧩 Architecture & Modules

### 1. 🌊 Axion Flow (Consumer Suite & Browser Extension)
* **Autonomous URL Sandbox:** Intercepts suspicious links and evaluates DOM structures in an isolated container to generate a real-time **Safety Score (0–100)**.
* **Live Traffic Inspector ("Burp Suite-Lite"):** Inspects incoming HTTP headers (CSP, HSTS) and tracking parameters on the fly.
* **Smart File Integrity Stalker:** Computes SHA-256 file hashes and strips malicious metadata before downloads touch local storage.
* **Credential Health Auditing:** Cross-references typed credentials securely against known breached databases using local k-anonymity hashing.

### 2. ⚡ Axion Prime (Enterprise Pentesting Suite)
* **Automated VAPT Engine:** Scans target web apps, API endpoints, and internal network maps for open ports and misconfigured services.
* **AI Exploit Simulator & Patch Recommender:** Audits code against OWASP Top 10 vulnerabilities, outputting automated reports with **ready-to-use secure code patches**.
* **API Fuzzer:** Floods backend routes with malformed payloads to test rate-limiting thresholds and JWT authorization bypasses.

### 3. 🛡️ Axion Force (Hardware Sentinel Node)
* **Inline Network Appliance:** Powered by a Raspberry Pi 5 / Zero 2W running passive packet analysis.
* **MitM & ARP Spoofing Interceptor:** Monitors gateway ARP tables in real time, instantly flashing warning LEDs and severing sockets if a Man-in-the-Middle attack occurs.
* **Physical Alert Display:** Integrates an SSD1306 OLED screen, status RGB LEDs, and a hardware panic button for instant network quarantine.

---

## 🛠️ Tech Stack

* **Frontend & Dashboards:** HTML5, JavaScript, Tailwind CSS
* **Browser Extension:** Manifest V3 API
* **Backend Core:** Python, FastAPI, Scapy, ONNX Runtime
* **Hardware Layer:** Raspberry Pi GPIO, Python C-bindings, I2C Display Drivers

---

## 📂 Repository Structure

```text
axion/
├── backend/          # FastAPI core engine, proxy routing, and sandbox logic
├── extension/        # Chrome Extension (Axion Flow - Manifest V3)
├── enterprise/       # VAPT scanner scripts & management dashboard UI
└── hardware/         # Raspberry Pi network sniffer & GPIO alert scripts (Axion Force)
