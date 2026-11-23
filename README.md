<div align="center">
  <a href="https://tinkeringdao.dev">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="assets/tinkeringdao-lockup-dark.png">
      <source media="(prefers-color-scheme: light)" srcset="assets/tinkeringdao-lockup-light.png">
      <img alt="TinkeringDao Labs" src="assets/tinkeringdao-lockup-dark.png" width="760">
    </picture>
  </a>
  <p>
    <a href="https://tinkeringdao.dev">tinkeringdao.dev</a> &middot;
    <a href="https://tinkeringdao.dev/log/">Field Journal</a> &middot;
    <a href="https://tinkeringdao.dev/brand/">Brand Kit</a> &middot;
    <a href="mailto:hello@tinkeringdao.dev">hello@tinkeringdao.dev</a>
  </p>
</div>

---

TinkeringDao Labs builds local-first open-source software, embedded firmware, and hardware interoperability tools where intelligence meets physical silicon: on-device speech, assistive cognition, and robotics safety latches (`llama.cpp`, `sherpa-onnx`, `IndicTrans2`, `SQLite`), `aarch64` embedded Linux and ARMv8 NEON runtimes, OpenWrt `24.10` hybrid wired/WDS meshes, sub-zero solar `868 MHz` LoRa repeaters, and clean-room macOS hardware drivers (`IOKit` DisplayPort AUX, `QCC5181` DSP). Built and measured on hardware benches in Bavaria, Germany and published gratuitously as non-commercial FOSS.

## Public Engineering Portfolio (`10` Repositories)

### On-Device Intelligence, Embedded Linux & Robotics

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`satori`](https://github.com/TinkeringDao/satori) | Offline Android voice recorder, streaming transcriber, Malayalam-to-English `IndicTrans2` reader, and local `llama.cpp` note/to-do synthesizer for standard displays and the Motorola Razr cover screen | Kotlin, C++, `sherpa-onnx`, `llama.cpp` |
| [`CiMind`](https://github.com/TinkeringDao/CiMind) | Local-first assistive cognition kernel: SHA-256 hash-chained SQLite audit ledger, 3-tier threshold action-intent policy evaluator, temporal memory client, melanopic EDI circadian lighting math, and Home Assistant / ESPHome blueprints | Python, SQLite, Home Assistant, ESPHome |
| [`actlatch`](https://github.com/TinkeringDao/actlatch) | Fail-closed SQLite actuator fault-latch recovery controller, offline simulation scaffold, and commissioning safety checklist for Reachy Mini Wireless | Python, SQLite |
| [`cronos64`](https://github.com/TinkeringDao/cronos64) | Native `aarch64` Go userspace runtime, ARMv8 NEON `int8` wake-word assembly, FDT v17 DTB memory/microphone patcher, thermal guard, and procedural 60 Hz display driver for unlocked MT8163 smart-display hardware (fork of [`HuskerMinion/techo5`](https://github.com/HuskerMinion/techo5)) | Go, ARM64 Assembly, Python, C |

### macOS Hardware Interoperability

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`auxpane`](https://github.com/TinkeringDao/auxpane) | Native macOS `IODPDevice` DisplayPort AUX (`DPCD 0x4B0..0x4FF`) volatile-SRAM `3840x1080` dual-monitor split controller and bezel-aware window manager for Synaptics `VMM5322` / Lenovo ThinkPad TB3 Dock Gen 2 (`40AN`) | C, `IOKit`, Swift, Python |
| [`biquadctl`](https://github.com/TinkeringDao/biquadctl) | Zero-daemon macOS Bluetooth RFCOMM (`BMAP`) 10-band parametric biquad NVRAM EQ and DSP calibration client, CoreAudio `HFP SCO` input guard, and B&K 5128 / Harman PEQ presets for Bose QuietComfort Ultra (`QCC5181`) | Objective-C, `IOBluetooth`, `CoreAudio`, Python |

### Mesh Networking, Sub-GHz LoRa Firmware & Upstream Contributions

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`firnmesh`](https://github.com/TinkeringDao/firnmesh) | Sub-zero solar Li-Ion MPPT power management, `< 1 uA` `P25Q16H` QSPI deep-sleep gating, `SX1262` front-end calibration, and DFU CLI for Seeed SenseCAP Solar Node P1-Pro (`nRF52840` + `SX1262`) | C++, PlatformIO, Python, KiCad |
| [`wdsweave`](https://github.com/TinkeringDao/wdsweave) | Clean-room OpenWrt `24.10` hybrid wired/WDS mesh provisioning toolkit, `QCA9563` / `QCA9886` hardware architecture notes, and deterministic UCI configuration generator for TP-Link Deco M4R / P9 nodes | Python, Shell, OpenWrt UCI |
| [`wadamesh`](https://github.com/TinkeringDao/wadamesh) | Touch-UI MeshCore LoRa companion firmware fork (`nRF52840` / `ESP32-S3`, `LR1110` / `SX1262`), including upstream Elecrow ThinkNode M9 contribution [`ALLFATHER-BV/wadamesh#826`](https://github.com/ALLFATHER-BV/wadamesh/pull/826) merged in `beta_103` | C++, PlatformIO, LVGL |
| [`meshcomod`](https://github.com/TinkeringDao/meshcomod) | MeshCore repeater and companion firmware builds (`ESP32` / `nRF52`) | C++, PlatformIO, LoRa |

Shared SHA-pinned GitHub Actions workflows, security gates, and community health templates live in [`TinkeringDao/.github`](https://github.com/TinkeringDao/.github).

## Prototyping & Component Support

Hardware prototyping, sensor/passive components, and developer infrastructure used across bench testing:

- [AISLER](https://aisler.net) for European ENIG PCB manufacturing and laser-cut stainless-steel SMD stencils.
- [ThirdReality](https://www.3reality.com) for Zigbee and Matter vibration (`3RVS01031Z`), motion, and night-pathway sensors in camera-free assistive living validation.
- [WAGO](https://www.wago.com) (`221 + Gelbox IPX8` splices and `2060` SMD terminals), [Coilcraft](https://www.coilcraft.com) (`XAL4020-222MEC` shielded power inductors), and [Samtec](https://www.samtec.com) (`TSW-110-07-G-S` interconnects).
- [LiveKit](https://livekit.io) (realtime WebRTC/SIP voice infrastructure) and [Composio](https://composio.dev) (structured tool integrations).

All repositories are published gratuitously as non-commercial FOSS (EU CRA `Regulation (EU) 2024/2847` Recitals 15 & 18; no paid consulting, commercial licensing, or paid support services). See [`LEGAL.md`](LEGAL.md) for statutory interoperability, trademark nominative fair use (`§ 23 Abs. 1 Nr. 3 MarkenG`), and German statutory notices.
