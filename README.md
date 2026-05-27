# ESP32 Template Repository

This repository is a production-ready ESP-IDF template for the ESP32 family. It is designed as a reusable starting point for new firmware projects with component-oriented architecture, OTA-ready partitioning, lightweight backlog management, and human-gated hardware-in-the-loop validation.

## Starting assumptions

- Framework: ESP-IDF.
- Initial targets: ESP32 family, with `esp32`, `esp32s2`, `esp32s3`, and future ESP32 variants treated as supported target classes.
- Languages: C and C++.
- Architecture: component-based firmware with a Board Abstraction Layer.
- Connectivity: Wi-Fi, BLE, Ethernet, MQTT, HTTP, and DALI-ready abstractions.
- OTA: A/B OTA baseline with explicit partition table.
- Configuration: `sdkconfig.defaults` plus component-level `Kconfig` files.
- Agent mode: balanced autonomy with safety gates.
- Documentation language: English.

## First local commands

```bash
idf.py set-target esp32
idf.py build
```

## Use as a project template

1. Create a new repository from this template on GitHub.
2. Clone the new repository to your local workspace.
3. Set target and build:

```bash
idf.py set-target esp32
idf.py build
```

## Repository contract

Codex and human contributors must read `AGENTS.md` before making changes. Scoped instructions exist in selected subdirectories and must be followed when working there.
