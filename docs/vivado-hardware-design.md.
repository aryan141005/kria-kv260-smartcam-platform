# Vivado Hardware Design

## 1. Overview

AMD Vivado was used in the hardware design workflow for the Kria KV260 SmartCam platform.

The objective of this stage was to configure the hardware platform, integrate the required processing and programmable logic components, and generate a hardware handoff for further development in Vitis.

## 2. Hardware Platform

The design targets the AMD Kria KV260 Vision AI Starter Kit, based on the Zynq UltraScale+ MPSoC architecture.

The platform combines:
- Processing System (PS)
- Programmable Logic (PL)
- Memory and high-speed interfaces
- Camera input and image-processing interfaces
- Display and video-processing connectivity

## 3. SmartCam Hardware Architecture

The reference hardware design uses the `kv260_ispMipiRx_vcu_DP` platform.

Its major functional blocks include:

- **Zynq UltraScale+ MPSoC:** Provides the processing system and programmable logic.
- **MIPI CSI-2 Receiver:** Receives image data from the camera interface.
- **Image Signal Processor (ISP):** Supports camera image-processing operations.
- **Video Codec Unit (VCU):** Provides video encoding and decoding functionality.
- **DisplayPort Interface:** Supports video output to an external display.
- **Memory Interfaces:** Enable data movement between hardware processing blocks and system memory.

## 4. Vivado Design Workflow

The high-level workflow consists of:

1. Open the KV260 hardware design project.
2. Configure the processing system and programmable logic.
3. Integrate the camera, image-processing, and video-related IP blocks.
4. Validate the hardware block design.
5. Generate the hardware design outputs.
6. Export the hardware platform as an XSA file.

## 5. XSA Hardware Handoff

The XSA (Xilinx Support Archive) contains hardware platform information required by downstream development tools.

It serves as the handoff between Vivado and Vitis, allowing the software development environment to use the configured hardware platform.

The exported XSA is an important input for subsequent platform configuration and acceleration development.

## 6. Development Tools

| Tool | Role |
|---|---|
| Vivado Design Suite | Hardware design and integration |
| IP Integrator | Block-level hardware integration |
| Hardware Validation | Design validation |
| XSA Export | Hardware handoff to Vitis |

## 7. Project Scope and Attribution

This document summarizes the Vivado hardware-design workflow and architecture described in the technical reference material.

It is documentation of the referenced development flow and should not be interpreted as a claim that every hardware block or design was independently created by the repository owner.
