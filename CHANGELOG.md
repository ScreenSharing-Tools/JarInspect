ChangeLog - vBeta ( 1.0 )

# DLL Activity Monitor - Release / Changelog

## Overview
Major update introducing a redesigned compact launch experience, standalone public distribution support, enhanced Windows App SDK runtime stability, and comprehensive startup diagnostics.

---

## What's New & Improved

### UI/UX & Splash Screen Redesign
- **Compact Loading Experience**: Redesigned the startup loading window (`MainWindow.xaml`) into a sleek, compact (`560x310`) modern card aesthetic.
- **Dynamic Progress Bar**: Replaced static placeholder images with a clean, smooth **0% -> 100% animated progress bar** that transitions seamlessly into the main dashboard.
- **Native & Premium Aesthetic**: Updated styling to feel native to modern Windows 11 with dark mode colors, refined borders, and polished typography.

---

## Fixes & Architecture

### WinUI 3 & Windows App SDK Startup Fixes
- **Resolved `MissingMethodException` (`SetEnvironmentVariable`)**: Upgraded Target Framework and SDK configuration to fully align with `.NET 10` (`net10.0-windows10.0.26100.0`).
- **Fixed Resource Lookup Crash (`0xc000027b`)**: Configured MSBuild targets (`CopyPriToTarget` & `CopyWinUIAssetsToPublish`) so that unpackaged MRT Core correctly finds `resources.pri` in both local `win-x64` and `publish` folders.
- **Runtime Self-Healing Check**: Added an automatic fallback in `Program.cs` that mirrors `JarInspect.pri` to `resources.pri` before XAML initialization if resources are missing.
- **Eliminated `CoreMessagingXP.dll` Collision (`0xc0000602`)**: Disabled duplicate bootstrap initialization (`WindowsAppSDKBootstrapInitialize=false`) and enabled `WindowsAppSDKUndockedRegFreeWinRTInitialize=true` for clean unpackaged self-contained runtime loading.

### Standalone Public Distribution
- **Self-Contained Deployment (`SelfContained=true`)**: Configured the build pipeline so end users **do not** need Visual Studio, the `.NET SDK`, or source code installed on their machines.
- **Ready-to-Run Binaries**: Distributed directly via the build output directory containing `JarInspect.exe` and its self-contained runtime dependencies.

### Diagnostic & Crash Logging
- **Custom Entry Point (`Program.cs`)**: Added an explicit `[STAThread]` entry point with global exception handlers (`UnhandledException`, `UnobservedTaskException`, and WinUI XAML exceptions).
- **Persistent Logs**: Application automatically records startup milestones to `jarinspect.log` and captures any unhandled fatal errors to `crash.log`.
