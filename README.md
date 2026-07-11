<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=2B2D31&height=200&section=header&text=JarInspect&fontSize=60&fontColor=ffffff&desc=Advanced%20Minecraft%20ScreenShare%20Tool&descFontSize=20&descAlignY=70" alt="JarInspect Banner"/>

<br>

<img src="https://img.shields.io/badge/Status-Beta-ED8B00?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white"/>
<img src="https://img.shields.io/badge/Built_By-@Sleepy-4F8CFF?style=for-the-badge&logo=github&logoColor=white"/>

<br><br>
</div>

> **JarInspect** is an advanced Minecraft screenshare tool designed specifically to catch cheaters. It provides deep visibility into client installations, allowing you to inspect Minecraft launchers, scan mod archives for tamper indicators, verify cryptographic signatures, and generate an itemized security assessment all inside a sleek, premium native desktop interface.

<br>
<hr>
<br>

## 🛠️ Built With

<div align="left">
  <img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white"/>
  <img src="https://img.shields.io/badge/.NET%208-512BD4?style=for-the-badge&logo=dotnet&logoColor=white"/>
  <img src="https://img.shields.io/badge/WinUI%203-0078D4?style=for-the-badge&logo=windows&logoColor=white"/>
  <img src="https://img.shields.io/badge/XAML-0C54C2?style=for-the-badge"/>
</div>

<br>

<br>
<hr>
<br>

## ✨ Core Features

<table width="100%">
  <tr>
    <td width="50%" valign="top">
      <h3>🛡️ Forensics & Security</h3>
      <ul>
        <li><b>Integrity Scoring:</b> Live 0 to 100 forensic score for any Minecraft instance.</li>
        <li><b>Itemized Deductions:</b> Transparent calculation breakdown explaining every score adjustment.</li>
        <li><b>Signature Validation:</b> Inspect cryptographic signatures (<code>META-INF/*.RSA</code>, <code>*.DSA</code>, <code>*.SF</code>).</li>
        <li><b>Tamper Detection:</b> Detect modified binaries, corrupt archives, and byte level mismatches.</li>
        <li><b>Bytecode Auditing:</b> Distinguish standard ProGuard mappings from suspicious code injection.</li>
        <li><b>Duplicate Shadowing:</b> Flag class namespace collisions across separate <code>.jar</code> archives.</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>🧭 Multi Launcher Intelligence</h3>
      <ul>
        <li><b>Universal Detection:</b> Automatically detects Vanilla, Prism, MultiMC, CurseForge, Modrinth, Lunar, Badlion, Feather, SKLauncher, ATLauncher, and Technic.</li>
        <li><b>Instance Exploration:</b> Inspect install paths, game directories, configurations, and mod folders.</li>
        <li><b>Instant Path Switching:</b> Seamlessly switch scan contexts directly to any discovered instance.</li>
        <li><b>Runtime Inspection:</b> Monitor active Java runtimes, command line arguments, and memory limits.</li>
      </ul>
    </td>
  </tr>
</table>

<br>
<hr>
<br>

## 📦 Mod & Server Analysis

| Feature | Description |
|---|---|
| 🔎 **API Cross Verification** | Verify local `.jar` hashes against official Modrinth database releases. |
| 🏷️ **Clean Categorization** | Clear distinction between `Verified` official mods, `Unknown` custom or unindexed archives, and `Modified` binaries. |
| 🌐 **Server Registry Parsing** | Parse local `servers.dat` NBT files to render real server icons, IPs, and join activity. |
