# <p align="center"><img src="https://omavsecurity.wordpress.com/wp-content/uploads/2026/09/cropped-omav_logo_round.png" alt="OmAV Security Suite" width="100" height="100" style="border-radius: 50%;" /><br>OmAV Security Suite</p>

<p align="center">
  <strong>Next-Gen Real-Time Antivirus & System Defense Powered by Native Rust.</strong><br>
  <em>Maximum Protection. Minimal Footprint. Zero Bloat.</em>
</p>

<p align="center">
  <a href="https://github.com/critmaths/omav-releases/releases/tag/v0.9.0-beta"><img src="https://img.shields.io/badge/Download-v0.9.0--beta-0284c7?style=for-the-badge&logo=windows&logoColor=white" alt="Download Beta" /></a>
  <a href="https://omavsecurity.wordpress.com/"><img src="https://img.shields.io/badge/Official_Website-Visit_Site-00d084?style=for-the-badge" alt="Official Website" /></a>
  <a href="https://patreon.com/omav"><img src="https://img.shields.io/badge/Patreon-Support_Project-f96854?style=for-the-badge&logo=patreon&logoColor=white" alt="Support on Patreon" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(64--bit)-0078D6?logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/Engine-Native%20Rust%20(Rayon%20Multi--core)-dea584?logo=rust" alt="Rust Engine" />
  <img src="https://img.shields.io/badge/Frontend-Flutter%20Desktop-02569B?logo=flutter" alt="Flutter Desktop" />
  <img src="https://img.shields.io/badge/License-Community%20Free%20%2F%20Commercial%20Pro-10b981" alt="License" />
</p>

---

## 💡 About OmAV

Tired of legacy antivirus suites consuming 15% of your CPU, gigabytes of RAM, and popping up intrusive ads while you work or game? 

**OmAV** is built from the ground up to solve this:
- **Core Native Engine:** Written in memory-safe, ultra-fast **Rust** with multi-threaded parallel file analysis via Rayon.
- **Zero-Day Heuristics:** Advanced Shannon entropy analysis, PE section inspection, direct NT syscall evasion detection, and Early Bird APC injection sentries.
- **Zero Background Lag:** Designed to protect your machine silently with negligible resource overhead.

---

## ⚡ Quick Download & Setup (Everyday Users)

> **No developer tools required.** OmAV ships as a standalone Windows installer under 16 MB.

1. **[Download OmAV-Setup-v0.9.0-beta.exe](https://github.com/critmaths/omav-releases/releases/download/v0.9.0-beta/OmAV-Setup-v0.9.0-beta.exe)**
2. Run the installer wizard and choose your installation directory.
3. Launch **OmAV** from your Start Menu or Desktop and run your first quick scan!

---

## 🛡️ Key Features

### 🚀 High-Speed Antivirus & Heuristic Defense
- **Multi-Core Parallel Scanner:** Scans thousands of files in seconds using Rayon worker threads.
- **Dual Heuristic & Signature Detection:** Combines MD5/SHA-256 database matching with dynamic Shannon entropy scoring to flag packed, encrypted, or disguised executables.
- **Advanced Evasion Sentry:** Detects direct NT syscalls (`NtAllocateVirtualMemory`, `NtWriteVirtualMemory`, `NtCreateThreadEx`), Early Bird APC queues, Process Hollowing, and AMSI/ETW memory blinding.
- **Real-Time Guard:** Actively watches drop zones, downloads, and temp folders to neutralize zero-day threats the moment they arrive.
- **Isolated Quarantine:** Safely encrypts and quarantines threats using AES-256-GCM.

### 🧰 Integrated Windows System Care
- **Registry Auditor & 1-Click Rollback:** Automatically inspects Windows registry hives for invalid references or orphaned keys, and creates safe `.reg` backup snapshots before applying any fixes.
- **Active Network Socket Sentry:** Audits all open TCP/UDP sockets, flags unverified remote connections, and terminates rogue listeners.
- **Safe Drive Cleaner:** Reclaims gigabytes of disk space by safely clearing temporary cache, orphaned crash dumps, and stale system logs.
- **Hardware-Encrypted Password Vault:** AES-256-GCM encrypted local vault with zero-knowledge master key protection.

---

## 💎 Plan Comparison

| Feature | Community Edition | OmAV Complete PRO |
| :--- | :---: | :---: |
| **High-Performance Rust Scanner** | ✅ Yes | ✅ Turbo Multi-Threaded |
| **On-Demand & Custom Folder Scans** | ✅ Yes | ✅ Yes |
| **Real-Time File Sentry** | ✅ Yes | ✅ Priority Real-Time Guard |
| **Advanced Zero-Day Heuristics** | ✅ Standard | ✅ Priority Cloud Stream |
| **Registry Snapshot & 1-Click Rollback** | ✅ Yes | ✅ Yes |
| **Network Sentry & Drive Optimizer** | ✅ Yes | ✅ Yes |
| **Password Vault & Secure Shredder** | ✅ Yes | ✅ Yes |
| **Pricing** | **100% Free Forever** | **$3.99/mo** • **$19.99/6mo** • **$34.99/yr** • **$49.99 Lifetime** |
| **Get Access** | [Download Free Beta](https://github.com/critmaths/omav-releases/releases/tag/v0.9.0-beta) | [Official Website & Store](https://omavsecurity.wordpress.com/#pricing) |

---

## 💻 System Requirements

- **Operating System:** Windows 10 or Windows 11 (64-bit architecture)
- **Processor:** 64-bit Intel, AMD, or ARM (x64 emulation)
- **RAM:** Minimum 512 MB (less than 60 MB RAM typical footprint)
- **Disk Space:** ~50 MB installed

---

## 🤝 Support, Community & Feedback

- 🌐 **Official Website:** [omavsecurity.wordpress.com](https://omavsecurity.wordpress.com/)
- 🐛 **Issue Tracker & False Positives:** [Open a GitHub Issue](https://github.com/critmaths/omav-releases/issues)
- 🧡 **Support the Project on Patreon:** [patreon.com/omav](https://patreon.com/omav)

<p align="center">
  <img src="https://github.com/user-attachments/assets/681ebaeb-80a1-4558-ab01-bf4004984474" alt="OmAV Banner" width="700" />
</p>

<p align="center">
  <em>© 2026 OmAV Security Suite. All rights reserved. Windows is a registered trademark of Microsoft Corporation.</em>
</p>