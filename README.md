# Wireshark Packet Analysis

**Project:** Network Packet Analysis using Wireshark  
**Author:** Sahil Rajesh Koli  
**Affiliation:** B.Tech (IT), D.Y. Patil University, Pune

---

## 📌 Project Overview
This project demonstrates basic network packet capture and analysis using **Wireshark**.  
The goal is to capture live traffic in a controlled lab environment, use filters to focus on relevant protocols, identify suspicious patterns, and document findings with screenshots and a short report.

---

## 🧰 Tools & Environment
- **Wireshark** (latest stable)  
- OS: Windows / Linux (Kali/Ubuntu)  
- Optional: VirtualBox with lab VMs (Kali Linux, Metasploitable)  
- Supporting files in this repo:
  - `report.docx` — detailed project report (https://drive.google.com/drive/folders/1E63qSG9odzkp8LpLg_j1Lld3MwTlJgzR?usp=drive_link)
  

---

## ⚙️ How to Reproduce (Step-by-step)

### 1. Setup
1. Install Wireshark from https://www.wireshark.org/  
2. (Optional) Set up lab VMs in VirtualBox on an isolated host-only/internal network:
   - Attacker: Kali Linux
   - Target: Metasploitable or intentionally vulnerable VM

### 2. Start a Capture
- Open Wireshark → select active network interface → Click **Start Capture**.

### 3. Generate Traffic (Examples)
- Browse a few websites from the target VM (HTTP/HTTPS).
- Run an `nmap` scan from attacker VM to target:
  ```bash
  nmap -sS -sV 192.168.56.101
