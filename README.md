# SmartCam Development on AMD Kria KV260

**Platform:** AMD Kria KV260 Vision AI Starter Kit  
**Tools & Technologies:** Vivado, Vitis, Zynq UltraScale+ MPSoC, PetaLinux, Yocto, BitBake, Embedded Linux

## Project Overview

This project focuses on the development and integration workflow of a SmartCam platform using the AMD Kria KV260 Vision AI Starter Kit.

The work explores the hardware and software development flow for an embedded vision platform, including FPGA hardware design, software development, embedded Linux configuration, and the associated build environment.

## Platform and Technologies

- **Hardware Platform:** AMD Kria KV260
- **Processing Architecture:** Zynq UltraScale+ MPSoC
- **Hardware Design:** Vivado Design Suite
- **Software Development:** Vitis
- **Embedded Operating System:** PetaLinux
- **Build System:** Yocto Project and BitBake
- **Software Components:** Device Tree Overlays and Embedded Linux

## Development Workflow

1. **Hardware Design:** Explore the hardware platform design and hardware handoff workflow using Vivado.
2. **Software Development:** Work with the Vitis development environment and exported hardware platform.
3. **Embedded Linux:** Explore PetaLinux project configuration and embedded Linux integration.
4. **Build System:** Study the Yocto/BitBake build workflow and associated dependencies.
5. **Platform Integration:** Organize the hardware and software components required for the SmartCam platform.

## Repository Structure

```text
kria-kv260-smartcam-platform/
├── README.md
├── docs/
├── hardware-design/
├── embedded-linux/
└── screenshots/
```

## Project Documentation

Detailed documentation, technical notes, and supporting material are organized in the respective directories.

## Note

This repository documents the development workflow and project artifacts that are available for sharing. Build completion and on-board functionality are reported only where supported by actual test evidence.

## Project Status

| Component | Status |
|---|---|
| Vivado hardware platform design | Documented |
| Hardware XSA export | Documented |
| Vitis platform development | Documented |
| DPU acceleration artifacts | Documented |
| Device tree overlay | Documented |
| PetaLinux configuration | Documented |
| Full PetaLinux build | Blocked by dependency-fetch errors |
| Board boot and runtime validation | Not verified |

## Project Documentation

Detailed technical documentation is available in the [`docs/`](docs/) directory.

## Screenshots and References

See [`screenshots/`](screenshots/) for reference design evidence and supporting visuals.
