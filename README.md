### 🛡️ JarInspect
> **Forensic & Intelligence Suite for Minecraft Environments**
> <img src="https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white"/> <img src="https://img.shields.io/badge/WinUI%203-0078D4?style=flat-square&logo=windows&logoColor=white"/>

A specialized desktop application designed for players, modpack developers, and security analysts to gain deep visibility into installations and runtime environments.

* **Cryptographic Auditing:** Scans `.jar` archives for valid signatures, detects tampering, and analyzes obfuscation mappings to flag unauthorized modifications or socket injections.
* **Dynamic Integrity Scoring:** Calculates a real-time (0–100) health score for any instance, backed by itemized deductions for shadowed packages or missing dependencies.
* **Launcher & Server Intelligence:** Automatically discovers instances across 11+ major launchers (Prism, MultiMC, Lunar, Feather, etc.) and parses local `servers.dat` NBT registries to extract IPs, rendered icons, and join history.
* **Premium Interface:** Wrapped in a sleek, responsive dark theme (`#0D0E12`) with smooth splash transitions and zero visual clutter.

<br>
<hr>
<br>

### ⚡ DLL Activity Monitor
> **Real-Time Windows Process & Module Tracker**
> <img src="https://img.shields.io/badge/C++17-00599C?style=flat-square&logo=cplusplus&logoColor=white"/> <img src="https://img.shields.io/badge/DirectX%2011-44CC11?style=flat-square&logo=windows&logoColor=white"/> <img src="https://img.shields.io/badge/ImGui-1C1C1C?style=flat-square"/>

A lightweight, high-performance desktop utility utilizing documented Windows APIs for diagnostics, visibility, and runtime analysis without memory dumping or process modification.

* **Live Process Attachment:** Hook into running processes via PID (with optional auto-attach for Minecraft) to track module loading, view persistent timestamps, and maintain an active session timeline.
* **Risk & Threat Analysis:** Cross-examine loaded modules with digital signature verification, SHA256 hash generation, and automated risk scoring while filtering out standard System DLLs.
* **Session Management:** Export discovered DLLs directly from disk, save monitoring sessions, and extract history logs for debugging or security reviews.
* **High-Performance UI:** Built on a clean, modern dark interface that refreshes instantly without resetting data, featuring organized tabs and live status indicators.
