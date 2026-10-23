# <p align="center"><img src="https://omavsecurity.wordpress.com/wp-content/uploads/2026/09/cropped-omav_logo_round.png" alt="OmAV Security Suite" width="100" height="100" style="border-radius: 50%;" /><br>OmAV Security Suite</p>

<p align="center">
  <strong>Next-Gen Real-Time Antivirus, System Care, WireGuard VPN Shield & Zero-Knowledge Vault.</strong><br>
  <em>Precision Engineering for Modern Defense by Critical Softworks</em>
</p>

<p align="center">
  <a href="https://github.com/critmaths/omav-releases/releases/latest"><img src="https://img.shields.io/badge/Download-v0.9.0--beta-0284c7?style=for-the-badge&logo=windows&logoColor=white" alt="Download Beta" /></a>
  <a href="https://omavsecurity.wordpress.com/"><img src="https://img.shields.io/badge/Official_Website-Visit_Site-00d084?style=for-the-badge" alt="Official Website" /></a>
  <a href="https://github.com/sponsors/critmaths"><img src="https://img.shields.io/badge/Sponsor-GitHub-ea4aaa?style=for-the-badge&logo=github&logoColor=white" alt="Sponsor on GitHub" /></a>
  <a href="https://patreon.com/omav"><img src="https://img.shields.io/badge/Patreon-Support_Project-f96854?style=for-the-badge&logo=patreon&logoColor=white" alt="Support on Patreon" /></a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(64--bit)-0078D6?logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/Engine-Native%20Rust%20(Rayon%20Multi--core)-dea584?logo=rust" alt="Rust Engine" />
  <img src="https://img.shields.io/badge/Frontend-Flutter%20Desktop-02569B?logo=flutter" alt="Flutter Desktop" />
  <img src="https://img.shields.io/badge/VPN-WireGuard%20ChaCha20--Poly1305-881337" alt="WireGuard VPN" />
  <img src="https://img.shields.io/badge/Vault-AES--256--GCM%20Zero--Knowledge-6366f1" alt="Vault" />
  <img src="https://img.shields.io/badge/Extension-Chrome%20%7C%20Edge%20%7C%20Firefox%20%7C%20Opera-a855f7" alt="Browser Extension" />
  <img src="https://img.shields.io/badge/License-Community%20Free%20%2F%20Commercial%20Pro-10b981" alt="License" />
</p>

---

## 💡 About OmAV

Tired of legacy antivirus suites consuming 15% of your CPU, gigabytes of RAM, and popping up intrusive ads while you work or game? 

**OmAV** is built from the ground up to solve this:
- **Core Native Engine:** Written in memory-safe, ultra-fast **Rust** with multi-threaded parallel file analysis via Rayon.
- **Zero-Day Heuristics:** Advanced Shannon entropy analysis, PE section inspection, direct NT syscall evasion detection, and Early Bird APC injection sentries.
- **Built-in VPN Shield:** High-speed encrypted WireGuard tunnel with specialized gaming, streaming, P2P, and privacy profiles.
- **Zero-Knowledge Vault & Browser Autofill:** AES-256-GCM encrypted passwords, payment cards, and identities with full extension autofill.
- **Zero Background Lag:** Designed to protect your machine silently with negligible resource overhead (<60 MB RAM).

---

## ⚡ Quick Download & Setup (Everyday Users)

> **No developer tools required.** OmAV ships as a standalone Windows installer under 16 MB.

1. **[Download Latest OmAV-Setup-v0.9.0-beta.exe](https://github.com/critmaths/omav-releases/releases/latest)**
2. Run the installer wizard and choose your installation directory.
3. Launch **OmAV** from your Start Menu or Desktop and run your first scan!

---

## 🛡️ Key Features

### 🚀 High-Speed Antivirus & Heuristic Defense
- **Multi-Core Parallel Scanner:** Scans thousands of files in seconds using Rayon worker threads.
- **Dual Heuristic & Signature Detection:** Combines MD5/SHA-256 database matching with dynamic Shannon entropy scoring to flag packed, encrypted, or disguised executables.
- **Advanced Evasion Sentry:** Detects direct NT syscalls (`NtAllocateVirtualMemory`, `NtWriteVirtualMemory`, `NtCreateThreadEx`), Early Bird APC queues, Process Hollowing, and memory blinding.
- **Real-Time Guard:** Actively watches drop zones, downloads, and temp folders to neutralize zero-day threats the moment they arrive.
- **Isolated Quarantine:** Safely encrypts and isolates threats using AES-256-GCM.

### 🌐 OmAV VPN Shield (WireGuard Encrypted Network Tunnel)
- **High-Speed ChaCha20-Poly1305 Tunnels:** Modern in-kernel WireGuard cryptography for maximum throughput and security.
- **Free 500 MB Test-Drive:** Test the VPN connection for free with zero credit card required.
- **Dedicated Exit Nodes:** Connect to high-speed dedicated servers (e.g. AWS Lightsail node at `100.29.30.198`).
- **4 Dedicated Tunnel Modes:**
  - 🎮 **Gaming & Low Latency:** Direct MTU clamping (1420 bytes) to eliminate packet fragmentation and drop ping times.
  - ⚡ **P2P & Fast Downloads:** Optimized TCP/UDP window buffers for torrenting and high-bandwidth downloads.
  - 🎬 **Streaming & 4K Media:** High-bitrate unbuffered pipeline for Netflix, YouTube, Disney+, and live sports.
  - 🛡️ **Ultra-Privacy & Ad-Block:** Network-wide DNS blocking of ad trackers, malware beacons, and fingerprinting scripts with strict Kill Switch.

### 🔑 Zero-Knowledge Password, Card & Identity Vault
- **AES-256-GCM Hardware-Level Encryption:** Hardware-encrypted local vault with PBKDF2 master key derivation.
- **Multi-Category Storage:** Dedicated tabs and models for **Website Logins**, **Credit/Debit Cards** (with CVV and masked preview), and **Addresses & Autofill Identities**.
- **1-Click Browser CSV Import:** Export from **Chrome, Edge, Firefox, Opera, or Bitwarden** as CSV and import all saved credentials into OmAV in seconds.
- **Cross-Browser Extension (Chrome, Edge, Opera, Firefox):**
  - **In-Field Shield Badge:** Discrete OmAV badge inside username and password fields for 1-click autofill.
  - **"Save to OmAV Vault?" Prompt:** Automatically captures submitted credentials and offers to protect them in your vault.
  - **"Switch to OmAV" Banner:** Smooth onboarding prompt to switch from your browser's unencrypted default password saving to OmAV.
  - **Cryptographic Password Generator:** Built-in 8–64 character entropy generator with customizable character sets.

### 🧰 Integrated Windows System Care
- **Registry Auditor & 1-Click Rollback:** Automatically inspects Windows registry hives for invalid references or orphaned keys, and creates safe `.reg` backup snapshots before applying any fixes.
- **Active Network Socket Sentry:** Audits all open TCP/UDP sockets, flags unverified remote connections, and creates 1-click Windows Firewall rules.
- **Deep Clean & Drive Optimizer:** Reclaims gigabytes of disk space by safely clearing temporary cache, orphaned crash dumps, and stale system logs.
- **System Stats Overlay:** Collapsible live HUD tracking CPU, GPU, RAM, active threads, and battery levels.

---

## 💎 Plan Comparison

| Feature | Community Free Edition | OmAV Complete PRO |
| :--- | :---: | :---: |
| **High-Performance Rust Scanner** | ✅ Yes | ✅ Turbo Multi-Threaded |
| **On-Demand & Custom Folder Scans** | ✅ Yes | ✅ Yes |
| **Real-Time File Sentry** | ✅ Yes | ✅ Priority Real-Time Guard |
| **Advanced Zero-Day Heuristics** | ✅ Standard | ✅ Priority Cloud Stream |
| **OmAV WireGuard VPN Shield** | 500 MB Free Test-Drive (US East) | ✅ **Unlimited Bandwidth (Dedicated 10Gbps Nodes)** |
| **VPN Tunnel Modes (Gaming/P2P/Streaming/Privacy)** | ✅ Standard | ✅ **Dedicated Priority Pipes** |
| **Password, Card & Identity Vault** | Basic Local View | ✅ **Full AES-256-GCM Vault** |
| **Browser Extension (Chrome/Edge/Firefox/Opera)** | ✅ Yes | ✅ **Full Autofill & Auto-Save Sync** |
| **1-Click Browser Password CSV Import** | ✅ Yes | ✅ **Unlimited Batch Import** |
| **Registry Snapshot & 1-Click Rollback** | ✅ Yes | ✅ Yes |
| **Network Sentry & Drive Optimizer** | ✅ Yes | ✅ Yes |
| **Cryptographic File Shredder** | ✅ Yes | ✅ Yes |
| **Floating System Stats HUD** | ✅ Yes | ✅ Yes |
| **Pricing** | **100% Free Forever** | **$3.99/mo** • **$19.99/6mo** • **$34.99/yr** • **$49.99 Lifetime** |
| **Get Access** | [Download Free Beta](https://github.com/critmaths/omav-releases/releases/latest) | [Official Website & Store](https://omavsecurity.wordpress.com/#pricing) |

---

## 💻 System Requirements

- **Operating System:** Windows 10 or Windows 11 (64-bit architecture)
- **Processor:** 64-bit Intel, AMD, or ARM (x64 emulation)
- **RAM:** Minimum 512 MB (less than 60 MB RAM typical footprint)
- **Disk Space:** ~50 MB installed

---

## 🤝 Community & Support

- **Bug Reports & Issues:** [GitHub Issues](https://github.com/critmaths/omav-releases/issues)
- **Official Website:** [omavsecurity.wordpress.com](https://omavsecurity.wordpress.com)
- **Support on Patreon:** [patreon.com/omav](https://patreon.com/omav)

---
*&copy; 2026 Critical Softworks. All rights reserved. Precision Engineering for Modern Defense.*
