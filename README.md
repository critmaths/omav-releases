<p align="center">
  <img src="omav_site_icon_squircle_512.png" alt="OmAV Infinity-Shield Logo" width="160" height="160" />
</p>

<h1 align="center">🛡️ OmAV Security Suite</h1>
<h3 align="center">Precision Windows Antivirus, 6-Layer Active Defense & Global WireGuard® VPN Shield</h3>

<p align="center">
  <b>Engineered by Critical Softworks</b><br/>
  <i>Next-generation endpoint protection combining high-performance Rust parallel heuristics, in-memory script de-obfuscation, decoy honeypot canary traps, and multi-peer zero-log WireGuard encryption.</i>
</p>

<p align="center">
  <a href="https://github.com/critmaths/omav-releases/releases"><img src="https://img.shields.io/github/v/release/critmaths/omav-releases?include_prereleases&color=00d2ff&label=Latest%20Release&logo=github" alt="Release" /></a>
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(64--bit)-0078D6?logo=windows&logoColor=white" alt="Windows" />
  <img src="https://img.shields.io/badge/Core%20Engine-Rust%202021%20(Rayon%20Multi--threaded)-dea584?logo=rust&logoColor=white" alt="Rust" />
  <img src="https://img.shields.io/badge/GUI-Flutter%203.24%20Desktop-02569B?logo=flutter&logoColor=white" alt="Flutter" />
  <img src="https://img.shields.io/badge/Active%20Defense-6--Layer%20Matrix%20(YARA%20%2B%20AMSI)-00ff9d" alt="Active Defense" />
  <img src="https://img.shields.io/badge/VPN-WireGuard%20(ChaCha20--Poly1305)-881337?logo=wireguard&logoColor=white" alt="WireGuard" />
  <img src="https://img.shields.io/badge/License-Community%20Free%20%7C%2014--Day%20Pro%20Trial-ffaa00" alt="License" />
</p>

---

## ⚡ Instant Download & Install

**Zero developer dependencies required.** No need to install Rust, Flutter, Python, or Git.

1. Download the verified release installer: [**`OmAV-Setup-v0.9.0-beta.exe`**](https://github.com/critmaths/omav-releases/releases/download/v0.9.0-beta/OmAV-Setup-v0.9.0-beta.exe) (~15.7 MB)
2. **Cryptographic SHA-256 Checksum**:
   ```text
   04bcf07a4ce9d371244b46f03133d45651ea65e9df80f92471e86602c891f0a8
   ```
3. Run the installer, launch **OmAV**, and immediately activate your **14-Day Free Pro Trial** with 1 click!

---

## 🚀 Key Architectural Pillars

### 1. 🛡️ 6-Layer Elite Active Defense Matrix
Commercial-grade, zero-marginal-cost protection running 100% on-device in native Rust:

1. **WinVerifyTrust Authenticode & PE Directory Inspection**: Calls Windows `wintrust.dll` with sub-millisecond offline caching (`WTD_CACHE_ONLY_URL_RETRIEVAL`) to verify OS trust chains. Automatically suppresses heuristic false positives on certified vendor binaries while elevating severity on tampered or forged PE `IMAGE_DIRECTORY_ENTRY_SECURITY` structures.
2. **YARA Multi-Pattern Byte & String Engine**: Inspects both case-insensitive ASCII and UTF-16LE wide strings across major threat families (`ShadowWiper`, `Mimikatz`, `CobaltStrike Beacon`, `AsyncRAT/Quasar`, `RedLine/Lumma Stealer`, `AMSI/ETW Patching`, `LockBit/BlackCat`, `ReverseShells`). All indicators are obfuscated at rest in `.rdata` to prevent host AV interference.
3. **Anti-Ransomware Canary Traps & Extension Sentry**: Automatically deploys hidden decoy honeypot vault guards (`.omav_canary_vault_guard.bak`) into watched folders. If any ransomware attempts unauthorized encryption or modification, OmAV immediately triggers an alert and re-arms the trap, while blocking 25+ known ransomware extensions (`.lockbit`, `.wannacry`, `.ryuk`, `.blackcat`, `.akira`).
4. **Live LOLBin Command-Line Sentinel**: Intercepts Living-Off-the-Land Binary abuse (`vssadmin delete shadows`, `wmic shadowcopy delete`, `bcdedit /set recoveryenabled no`, `certutil -urlcache`, `regsvr32 /s /u /i:http`, `mshta javascript:`).
5. **AMSI & Script De-Obfuscator**: Normalizes PowerShell backtick (`` ` ``) and caret (`^`) obfuscation, de-concatenates nested strings (`'Amsi'+'Utils'`), automatically unpacks Base64 UTF-16LE (`-EncodedCommand`) and UTF-8 payloads directly in memory, and inspects decoded execution buffers.
6. **Live Threat Intelligence Delta Sync**: 1-click sync pulling verified recent SHA-256 malware signatures directly from `abuse.ch` MalwareBazaar and deduplicating them into local storage.

---

### 2. 🌐 32-City Multi-Peer Global WireGuard® VPN Network
- **Kernel-Level WireGuard Performance**: ChaCha20-Poly1305 symmetric encryption for maximum bandwidth, lower ping, and minimal CPU overhead.
- **32 Global Metros Across 19 Countries**:
  - **Americas (14 Cities)**: Virginia (US East Gateway), New York City, Miami, Chicago, Dallas, Los Angeles, Seattle, Oregon, Toronto, Montreal, Vancouver, Mexico City, São Paulo, Buenos Aires.
  - **Europe (11 Cities)**: London, Manchester, Dublin, Frankfurt, Berlin, Amsterdam, Paris, Zurich (Privacy Vault), Stockholm, Madrid, Milan.
  - **Asia-Pacific & Middle East (7 Cities)**: Tokyo, Osaka, Seoul, Singapore, Sydney, Mumbai, Dubai.
- **Dynamic Multi-Peer Subnet Management**: Automated server daemon assigns unique `/32` IP leases (`10.8.0.3` to `10.8.254.254`) via Linux kernel hot-reloading with zero tunnel downtime.
- **4 Dedicated Tunnel Profiles**:
  - 🎮 **Gaming & Low Ping**: Clamped 1420 MTU buffer and direct fast-path routing to eliminate jitter.
  - ⚡ **P2P & Fast Downloads**: Optimized TCP/UDP window buffers for maximum throughput.
  - 🎬 **Streaming & 4K Media**: High-bitrate unbuffered pipeline for Netflix, YouTube, and sports.
  - 🛡️ **Ultra-Privacy & Ad-Block**: Zero-log DNS sinkhole for trackers and malware with a hard Kill Switch.

---

### 3. 🔑 Zero-Knowledge Password, Card & Identity Vault
- **AES-256-GCM Cryptographic Storage**: Local zero-knowledge credential vault protected by PBKDF2 (100,000 iterations) and memory zeroization.
- **Multi-Record Management**: Store **Logins**, **Payment Cards** (with CVV, expiration, and masked numbers), and **Addresses & Identities**.
- **1-Click Browser CSV Import**: Seamless migration from **Google Chrome, Microsoft Edge, Mozilla Firefox, Opera, and Bitwarden**.
- **Cross-Browser Extension (`browser-extension/`)**:
  - Manifest V3 extension compatible with **Chrome, Edge, Brave, Opera, and Firefox**.
  - In-field shield autofill badge on login and credential inputs.
  - Automatic **"Save password to OmAV Vault?"** prompt on submission.
  - Built-in 8–64 character cryptographic password generator.

---

### 4. 🧰 Integrated Windows Optimization & Maintenance
- **Registry Snapshot & 1-Click Rollback**: Create point-in-time system state backups before installing software or running deep cleans.
- **Active Process & Network Sentry**: Real-time process inspection with 1-click Windows Firewall rule creation.
- **Safe Drive Cleaner**: Clean temporary clutter, cache, and stale logs without risking system stability.
- **Cryptographic File Shredder**: Multi-pass secure file wiper with Windows Explorer context menu integration.
- **System Stats HUD Overlay**: Collapsible live HUD tracking CPU, GPU, RAM, active threads, and battery levels.

---

### 5. 🔄 Cryptographic Auto-Updater & CDN Architecture
- **Zero-Egress Distribution**: Hosted across GitHub Raw CDN, GitHub Releases API, and the AWS Control Node.
- **In-Memory SHA-256 Verification**: Verifies downloaded installer packages against the signed [update_manifest.json](update_manifest.json) before execution.
- **1-Click Silent Update**: Automatically launches the verified installer with `/SILENT /CLOSEAPPLICATIONS /RESTARTAPPLICATIONS`.

---

## 💎 Edition Comparison

| Capability | Community Free | Pro 14-Day Free Trial | OmAV Complete Pro |
| :--- | :---: | :---: | :---: |
| **Rust Multi-Threaded Engine** | ✅ Yes | ✅ Yes (Turbo) | ✅ Yes (Turbo) |
| **6-Layer Active Defense Matrix** | ✅ Yes | ✅ Yes | ✅ Yes |
| **WinVerifyTrust & YARA Engine** | ✅ Yes | ✅ Yes | ✅ Yes |
| **Ransomware Canaries & Extension Guard** | ✅ Yes | ✅ Yes | ✅ Yes |
| **LOLBin & AMSI De-Obfuscator** | ✅ Yes | ✅ Yes | ✅ Yes |
| **Live MalwareBazaar Threat Sync** | ✅ Yes | ✅ Priority Stream | ✅ Priority Stream |
| **WireGuard® VPN Shield** | 500 MB Free Test-Drive | ✅ **Unlimited Bandwidth** | ✅ **Unlimited Bandwidth** |
| **32 Global City Exit Nodes** | Virginia Gateway | ✅ **All 32 Global Metros** | ✅ **All 32 Global Metros** |
| **VPN Tunnel Modes (Gaming/P2P/Streaming)** | ✅ Standard | ✅ **Priority Pipes** | ✅ **Priority Dedicated** |
| **Zero-Knowledge Password Vault** | Read-Only | ✅ **Full AES-256-GCM** | ✅ **Full AES-256-GCM** |
| **Browser Extension Autofill** | ✅ Yes | ✅ **Full Sync** | ✅ **Full Sync** |
| **1-Click Windows Firewall Blocking** | — | ✅ **Included** | ✅ **Included** |
| **Price** | **$0 Free Forever** | **$0 for 14 Days** | **$3.99/mo** or **$34.99/yr** |

---

## 🛠️ Developer Setup & Building from Source

### Prerequisites
- [Rust & Cargo](https://www.rust-lang.org/tools/install) (1.75+)
- [Flutter SDK](https://flutter.dev/docs/get-started/install) (3.24+) with Windows Desktop enabled
- [Inno Setup 6](https://jrsoftware.org/isdl.php) (for packaging the single-file installer)

### 1-Click Release Build Pipeline
Run the unified PowerShell release packaging script:
```powershell
.\build_release.ps1
```
This automatically:
1. Compiles `engine/` into an optimized release DLL (`antivirus_engine.dll`).
2. Builds the obfuscated Flutter Windows desktop application.
3. Bundles embedded WireGuard binaries (`wireguard.exe`, `wg.exe`) and signatures.
4. Generates `dist/OmAV-Setup-v0.9.0-beta.exe` and outputs the signed `update_manifest.json`.

### Running Unit & Widget Tests
```powershell
# Run Rust Engine unit tests (41 tests)
cd engine
cargo test --lib

# Run Flutter GUI widget tests (57 tests)
cd ../frontend
flutter test
```

---

## 🤝 Community, Support & Links
- **Download Latest Installer**: [GitHub Releases](https://github.com/critmaths/avprog/releases)
- **Submit Bug Reports & Ideas**: [GitHub Issues](https://github.com/critmaths/avprog/issues)
- **Official Website & Docs**: [omavsecurity.wordpress.com](https://omavsecurity.wordpress.com)
- **Support Independent Development**: [Patreon](https://patreon.com/omav)

---

<p align="center">
  <b>© 2026 Critical Softworks. All rights reserved.</b><br/>
  <i>Engineered with Rust, Flutter, and WireGuard for unapologetic Windows security and privacy.</i>
</p>
