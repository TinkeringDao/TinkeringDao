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

TinkeringDao Labs builds local-first software, firmware, and electronics where intelligence meets physical hardware—from on-device speech and vision models (`llama.cpp`, `sherpa-onnx`, `IndicTrans2`, `BioCLIP-2`), solar `868 MHz` LoRa meshes, and `MPTCP` multi-WAN networking to robotics safety latches (`Reachy` / `ROS 2`), Color E-Ink framebuffers, and clean-room device drivers (`IOKit` DisplayPort AUX, `QCC5181` DSP). Measured on real benches in Bavaria, Germany and published as open source.

## Public Repositories

### On-Device Speech & Robotics

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`satori`](https://github.com/TinkeringDao/satori) | Offline Android voice recorder, streaming transcriber, Malayalam-to-English `IndicTrans2` reader, and local `llama.cpp` note/to-do synthesizer for standard displays and the Motorola Razr cover screen | Kotlin, C++, `sherpa-onnx`, `llama.cpp` |
| [`reachy-companion`](https://github.com/TinkeringDao/reachy-companion) | Offline simulation scaffold, SQLite fault-latch recovery controller, and commissioning checklist for Reachy Mini Wireless | Python, SQLite |

### macOS Hardware Interoperability

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`stretch-the-mac`](https://github.com/TinkeringDao/stretch-the-mac) | macOS `IODPDevice` DisplayPort AUX (`DPCD 0x4B0..0x4FF`) ViewXpand `3840x1080` split controller and bezel-aware dual-monitor window snapper for the Lenovo ThinkPad TB3 Dock Gen 2 (`Synaptics VMM5322`) | C, `IOKit`, Swift, Python |
| [`Woke-Bose`](https://github.com/TinkeringDao/Woke-Bose) | macOS Bluetooth RFCOMM (`BMAP`) NVRAM/DSP calibration client, CoreAudio `HFP SCO` input guard, and B&K 5128 / Harman PEQ presets for Bose QuietComfort Ultra Headphones (`QCC5181`) | Objective-C, `IOBluetooth`, `CoreAudio`, Python |

### Sub-GHz LoRa Mesh Firmware & Upstream Contributions

| Repository | Focus | Stack |
| :--- | :--- | :--- |
| [`sensecap-solar-p1-pro-unleashed`](https://github.com/TinkeringDao/sensecap-solar-p1-pro-unleashed) | Solar repeater firmware and DFU CLI for Seeed SenseCAP Solar Node P1-Pro (`nRF52840` + `SX1262`): `CN3165` MPPT cold-weather load shedding and `P25Q16H` QSPI deep-sleep power gating | C++, PlatformIO, Python |
| [`wadamesh`](https://github.com/TinkeringDao/wadamesh) | Touch-UI MeshCore LoRa firmware fork (`nRF52840` / `ESP32-S3`, `LR1110` / `SX1262`), including upstream Elecrow ThinkNode M9 contribution [`ALLFATHER-BV/wadamesh#826`](https://github.com/ALLFATHER-BV/wadamesh/pull/826) merged in `beta_103` | C++, PlatformIO, nRF52840 / ESP32-S3, LR1110 / SX1262 |
| [`meshcomod`](https://github.com/TinkeringDao/meshcomod) | MeshCore repeater and companion firmware builds (`ESP32` / `nRF52`) | C++, PlatformIO, LoRa |

## Hardware, Manufacturing & Ecosystem Partners

Our open-source hardware prototypes, PCB layouts, and edge-AI integrations are supported by:

- **[AISLER](https://aisler.net)** — European ENIG PCB manufacturing and laser-cut stainless-steel SMD stencils.
- **[PCBWay](https://www.pcbway.com)** — Multi-layer PCB/PCBA prototyping and CNC 6061 aluminum enclosures.
- **[ThirdReality](https://www.3reality.com)** — Zigbee/Matter vibration (`3RVS01031Z`), motion, and night-pathway sensors for camera-free assistive living.
- **[WAGO](https://www.wago.com)** (`221 + Gelbox IPX8` & `2060` SMD terminals), **[Coilcraft](https://www.coilcraft.com)** (`XAL4020-222MEC` shielded power inductors), and **[Samtec](https://www.samtec.com)** (`TSW-110-07-G-S` interconnects).
- **[Heltec Automation](https://heltec.org)** (`Mesh Node T114 V2.0` & `Vision Master E213`) and **[Volla Systeme](https://volla.online)** ([`github.com/hellovolla`](https://github.com/hellovolla) — `Volla OS` & `Volla Supportive Intelligence`).
- **[LiveKit](https://livekit.io)** (Realtime WebRTC/SIP voice infrastructure), **[Composio](https://composio.dev)** (Agentic MCP integrations), and **[JetBrains](https://www.jetbrains.com/?from=TinkeringDao)** (CLion, RustRover, PyCharm).

See [`LEGAL.md`](LEGAL.md) for statutory interoperability, trademark nominative fair use, non-commercial FOSS, and German statutory notices.
