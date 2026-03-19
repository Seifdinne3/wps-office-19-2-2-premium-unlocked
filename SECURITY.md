# Security Policy

## Supported Versions

Use this section to tell people about which versions of your project are
currently being supported with security updates.

| Version | Supported          |
| ------- | ------------------ |
| 5.1.x   | :white_check_mark: |
| 5.0.x   | :x:                |
| 4.0.x   | :white_check_mark: |
| < 4.0   | :x:                |

## Reporting a Vulnerability

Use this section to tell people how to report a vulnerability.

Tell them where to go, how often they can expect to get an update on a
reported vulnerability, what to expect if the vulnerability is accepted or
declined, etc.

# 🛡️ SECURITY ALERT: Malicious "WPS Unlocker" & "Premium" ZIP Trap
**Threat Level:** 🔴 CRITICAL (Active Data Stealer)
**Detected Malware:** Trojan:Win32/Alevaul!rfn

---

### 📝 Executive Summary
A malicious campaign is targeting users interested in **WPS (Wi-Fi Protected Setup) hacking** and **Premium Office software**. Attackers are uploading `.zip` files to GitHub without any source code, masking a sophisticated Trojan designed to bypass security and steal sensitive data.

---

### 🔍 1. The Trap: WPS Exploitation Lure
The attacker uses "Social Engineering" by offering tools to exploit the 8-digit PIN vulnerability in WPS-enabled routers (WPA/WPA2).
* **The Bait:** A ZIP file claiming to be a "WPS Crack" or "WPS Office Premium Unlocked".
* **The Red Flag:** The repository contains **NO Source Code**—only a compiled "Black Box" binary inside a ZIP.



---

### ☣️ 2. The Core Threat: Trojan:Win32/Alevaul!rfn
Once the file inside the ZIP is executed, the **Alevaul** Trojan initiates:
* **Credential Harvesting:** It steals saved passwords and active session cookies from Chrome, Edge, and Firefox to bypass 2FA.
* **Financial Theft:** It scans for Crypto wallets (MetaMask, Bitcoin) and banking session data.
* **Persistent Access:** It injects itself into the **Windows Registry** and `AppData` to survive system reboots.
* **Backdoor (RAT):** It establishes a connection to a Command & Control (C2) server, allowing hackers to upload Ransomware.



---

### 📊 Risk Assessment Table
| Feature | Status | Risk Level |
| :--- | :--- | :--- |
| **Source Code** | ❌ Missing | **Critical** (No Transparency) |
| **Delivery Method** | 📦 ZIP File | **High** (Detection Evasion) |
| **Payload Type** | 🦠 Alevaul | **Critical** (Full Data Theft) |
| **Persistence** | ✅ Active | **High** (Registry Infection) |

---

### 🛡️ Mandatory Safety Steps
1. **DO NOT EXTRACT:** Delete any ZIP from GitHub that doesn't provide inspectable source code.
2. **SCAN OFFLINE:** If infected, run **Microsoft Defender Offline Scan** immediately.
3. **RESET CREDENTIALS:** Change all passwords (Email, Banking, Social Media) from a **different, clean device**.
4. **DISABLE WPS:** To prevent the very hack this tool promised, manually disable WPS in your router settings.



---
**📢 Please share this to protect the community from GitHub-hosted malware.**
