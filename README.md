# TinkeringDao

Systems engineering across Sub-GHz LoRa mesh firmware, Android/macOS hardware-protocol interoperability, robotics, and on-device speech/ML inference. Most projects here come from fixing practical gaps in hardware I use daily, from bare-metal/RTOS power management on constrained radios to clean-room macOS drivers and offline mobile apps without cloud dependencies. Code is published as independent, non-commercial open source.

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

See [`LEGAL.md`](LEGAL.md) for statutory interoperability, trademark nominative fair use, non-commercial FOSS, and German statutory notices.
