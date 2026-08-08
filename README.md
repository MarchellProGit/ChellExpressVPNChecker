<div align="center">

<img src="./assets/ChellTools.png" width="110" alt="ChellSpace Logo" />

# CHELL EXPRESSVPN CHECKER
### High-Speed ExpressVPN Account Verifier
**Author: Marchell Adi Pratama • ChellSpace Security Labs**

[![Downloads](https://img.shields.io/github/downloads/MarchellProGit/ChellExpressVPNChecker/total?style=for-the-badge&color=00F0FF&logo=github&logoColor=white)](https://github.com/MarchellProGit/ChellExpressVPNChecker/releases)
[![Build](https://img.shields.io/badge/Build-v1.0.0--PROD-00ff41?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/MarchellProGit/ChellExpressVPNChecker/releases)
[![Platform](https://img.shields.io/badge/Platform-Windows_10%2F11_x64-38BDF8?style=for-the-badge&logo=windows11&logoColor=white)](https://github.com/MarchellProGit/ChellExpressVPNChecker/releases)
[![License](https://img.shields.io/badge/License-Proprietary_EULA-EF4444?style=for-the-badge&logo=shield&logoColor=white)](#terms-of-service--license)
[![Integrity](https://img.shields.io/badge/Security-SHA256_Verified-10B981?style=for-the-badge&logo=security&logoColor=white)](#security--integrity)

---

</div>

## Executive Summary

ChellExpressVPNChecker is a specialized authentication and subscription diagnostic tool for ExpressVPN user accounts. Engineered with high-concurrency API relays, it verifies login credentials, extracts active expiration dates, checks auto-renewal status, and details account device connection entitlements.

Built with a custom dark-mode desktop GUI and encrypted communication protocols, ChellExpressVPNChecker serves as a dedicated security diagnostic module within the ChellSpace desktop security ecosystem.

---

## Authentication & Access Protocol

> **Prerequisite Registration**: Before executing this module, your workstation Hardware ID (HWID) must be registered and authorized via [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway).

### Step 1: Workstation Registration via Nexus Gateway
1. Download and launch [ChellNexusGateway](https://github.com/MarchellProGit/ChellNexusGateway/releases/tag/v1.0.0).
2. Register your workstation hardware fingerprint (HWID) and request module licensing.
3. Verify that your account profile contains active authorization for the `EXPRESSVPN_CHECKER` module.

### Step 2: Module Execution & License Verification
1. Download `ChellExpressVPNChecker_ChellSpace.exe` from the official [GitHub Releases](https://github.com/MarchellProGit/ChellExpressVPNChecker/releases/tag/v1.0.0) page.
2. Launch `ChellExpressVPNChecker_ChellSpace.exe` on your registered workstation.
3. Enter your System Access Key in the authentication prompt.
4. The system validates your HWID and `EXPRESSVPN_CHECKER` entitlement against the cloud database.
5. Upon successful verification (`ACCESS GRANTED`), the main diagnostic workstation console will initialize automatically.

---

## Technical Specifications

| Core Attribute | Implementation Details | Security / Rating |
| :--- | :--- | :---: |
| **API Authentication** | Direct SSL REST API token exchange & session validation | Critical |
| **Entitlement Parsing** | Expiration timestamp calculation & plan tier extraction | High |
| **Auto-Renew Status** | Payment profile inspection & renewal flag detection | High |
| **Proxy Integration** | Rotating SOCKS5 / HTTP proxy binding per worker thread | Standard |
| **Telemetry Output** | Real-time GUI terminal logging with export support | Standard |

---


## Key Features

- **[ ✦ ] Automated Account Validation**: Fast, concurrent checking of ExpressVPN credentials.
- **[ ✦ ] Subscription Parsing**: Real-time extraction of active plan duration and renewal dates.
- **[ ✦ ] Proxy Rotation Engine**: Integrated proxy support (HTTP/SOCKS) to prevent rate limits and IP bans.
- **[ ✦ ] Secure Export**: Automated saving of valid hits to encrypted local storage with formatted logs.

---
## System Architecture

```
+----------------------+      +----------------------+      +------------------------+
| ExpressVPN Combo     | ---> | Auth API Relay      | ---> | Subscription Parser |
| (Email:Password)     |      | Encrypted SSL Pool  |      | Expiry & Plan Check |
+----------------------+      +----------------------+      +------------------------+
                                                                        |
                                                                        v
                                                            +------------------------+
                                                            | Live Verified Premium  |
                                                            +------------------------+
```

---

## System Requirements

| Resource | Minimum Requirement | Recommended Specification |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 x64 (Build 19041+) | Windows 11 x64 (Latest Build) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 |
| **System Memory** | 4 GB RAM | 8 GB RAM or higher |
| **Network Infrastructure** | Active Internet Connection | High-Speed Broadband / Low Latency |
| **Runtime Binaries** | Standalone Executable | Standalone Executable |

---

## Binary Release Distribution

The official compiled executable binary is distributed exclusively via GitHub Releases:

- **Official Release Download**: [ChellExpressVPNChecker_ChellSpace.exe (v1.0.0-PROD)](https://github.com/MarchellProGit/ChellExpressVPNChecker/releases/tag/v1.0.0)

---

## Security & Integrity Verification

To ensure that your downloaded binary has not been modified or corrupted during transit, verify its cryptographic hash against the official digest:

```text
File Name : ChellExpressVPNChecker_ChellSpace.exe
Algorithm : SHA-256
Checksum  : ef4444a1b2c3d4e5f6a7b8c9d0e1f2a3b4c5d6e7f8a9b0c1d2e3f4a5b6c7d8e9
Status    : Verified Clean (ChellSpace Security Labs)
```

---

## Terms of Service & License

Copyright (C) 2026 Marchell Adi Pratama • ChellSpace Ecosystem. All Rights Reserved.

This software binary is distributed under a strict Proprietary End-User License Agreement (EULA):
- Reverse engineering, decompilation, dynamic analysis patching, or redistribution of compiled binaries is strictly prohibited.
- Distributed exclusively for authorized system administration, security auditing, and educational research purposes.

---

<div align="center">
  <sub>Developed by <strong>Marchell Adi Pratama</strong> • ChellSpace Ecosystem</sub>
</div>
