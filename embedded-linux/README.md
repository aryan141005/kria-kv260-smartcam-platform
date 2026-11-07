# Embedded Linux Development

This directory contains documentation related to the embedded
Linux software development flow for the AMD Kria KV260 platform.

Technologies and tools:
- PetaLinux
- Yocto Project
- BitBake
- Device Tree Overlays
- Embedded Linux Build System

Topics:
- PetaLinux project configuration
- Yocto build workflow
- Device tree configuration
- Linux image generation
# Embedded Linux

This directory is intended to organize embedded Linux configuration details and supporting technical evidence for the AMD Kria KV260 SmartCam platform.

## Planned Contents

- PetaLinux project configuration files, where available.
- Device-tree source files (`.dts` and `.dtsi`).
- Device-tree overlays (`.dtbo`).
- FPGA Manager configuration details.
- Yocto and BitBake build configuration.
- Build logs and error analysis.
- Embedded Linux deployment documentation.

## Embedded Linux Workflow

The documented workflow covers:

1. PetaLinux project setup using the KV260 BSP.
2. Hardware platform integration.
3. Device-tree generation.
4. FPGA Manager and overlay integration.
5. Yocto and BitBake dependency processing.
6. Embedded Linux image generation.

## Build Status

The reference workflow reached the PetaLinux build stage but encountered seven dependency-fetch failures.

A successful final Linux image build and on-board deployment have not been verified.

## Repository Guidelines

Only genuine project files and evidence that are available and permitted for publication should be added.

Do not upload credentials, proprietary files, or third-party source code without appropriate permission.

This directory currently serves as an organizational structure for embedded Linux documentation and evidence.
