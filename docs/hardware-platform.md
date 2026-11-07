# Hardware Platform – AMD Kria KV260

## 1. Overview

The AMD Kria KV260 Vision AI Starter Kit is an FPGA-based development platform designed for embedded vision and AI applications.

It is built around the K26 System-on-Module (SOM), which integrates a Zynq UltraScale+ MPSoC. The platform combines programmable logic (PL) with an Arm-based processing system (PS), enabling hardware acceleration alongside embedded software execution.

## 2. Platform Components

### Kria K26 System-on-Module

The K26 SOM provides the primary processing and programmable logic resources required for the SmartCam platform.

Key features:
- Zynq UltraScale+ MPSoC architecture
- Arm-based processing system
- Programmable logic for hardware acceleration
- External memory and high-speed interfaces

### KV260 Carrier Card

The KV260 carrier card provides connectivity and peripheral interfaces for the K26 SOM.

It supports camera, display, networking, and other peripheral connections required for embedded vision applications.

## 3. Processing Architecture

The platform consists of two major processing domains:

**Processing System (PS)**
- Runs embedded Linux.
- Handles application-level processing and system management.
- Provides communication between software and programmable logic.

**Programmable Logic (PL)**
- Implements custom hardware functionality.
- Supports camera data acquisition and processing pipelines.
- Enables hardware acceleration for vision-related workloads.

## 4. SmartCam Hardware Data Flow

The SmartCam architecture uses the following high-level data flow:

1. Camera input provides image data to the platform.
2. The MIPI CSI-2 interface receives camera data.
3. The ISP processes the incoming image stream.
4. The hardware pipeline transfers data through the programmable logic and memory interfaces.
5. Processing and acceleration components support vision workloads.
6. Processed data can be directed toward display or network-based output.

## 5. Development Tools

The hardware development workflow uses:

| Tool | Purpose |
|---|---|
| AMD Vivado | Hardware design and bitstream generation |
| AMD Vitis | Platform and acceleration development |
| XSCT / HSI | Hardware handoff and device-tree generation |
| Device Tree Compiler (DTC) | Device-tree compilation |

## 6. Hardware Design Handoff

The Vivado hardware design is exported as an XSA (Xilinx Support Archive).

This hardware handoff is used by Vitis and other development tools to configure the software platform and generate the required hardware-related outputs.

## 7. Scope and Attribution

This document describes the hardware platform and architecture based on the technical reference material used for this project.

It is intended as technical documentation and a learning reference. It does not claim that every component or implementation described here was independently developed by the repository owner.
