# Project Overview

## SmartCam Development on AMD Kria KV260

### 1. Introduction

The AMD Kria KV260 Vision AI Starter Kit is an embedded development platform designed for vision and AI applications. It combines a Zynq UltraScale+ MPSoC with programmable logic, enabling hardware acceleration alongside embedded software execution.

This project explores the development flow for the SmartCam application on the Kria KV260 platform, covering hardware design, acceleration platform development, device-tree integration and embedded Linux configuration.

### 2. Project Objectives

The main objectives are:

- Understand the hardware architecture of the AMD Kria KV260.
- Explore the Vivado hardware design and XSA export workflow.
- Understand Vitis platform generation and accelerator kernel integration.
- Study FPGA acceleration overlay generation.
- Explore device-tree overlay generation and compilation.
- Configure the PetaLinux environment for the SmartCam application.
- Understand the Yocto and BitBake build process.

### 3. Hardware Platform

**Target platform:** AMD Kria KV260 Vision AI Starter Kit

**Processing architecture:** Zynq UltraScale+ MPSoC

The platform combines:
- Processing System (PS)
- Programmable Logic (PL)
- MIPI CSI-2 camera interface
- Image Signal Processing (ISP)
- Video Codec Unit (VCU)
- DisplayPort video output

### 4. Software Tools and Technologies

| Tool / Technology | Purpose |
|---|---|
| Vivado Design Suite | Hardware platform design |
| Vitis | Platform and accelerator development |
| XSCT / HSI | Hardware software interface and device-tree generation |
| Device Tree Compiler | Device-tree overlay compilation |
| Bootgen | Bitstream conversion |
| PetaLinux 2022.1 | Embedded Linux configuration |
| Yocto Project | Embedded Linux build framework |
| BitBake | Recipe-based build and dependency management |

### 5. Development Flow

The SmartCam development workflow consists of the following stages:

1. Hardware platform design and XSA generation using Vivado.
2. Vitis platform generation and accelerator kernel compilation.
3. FPGA acceleration overlay preparation.
4. Device-tree overlay generation and compilation.
5. PetaLinux project configuration.
6. Embedded Linux build using Yocto and BitBake.

### 6. Project Status

The referenced project documentation reports completion of the Vivado hardware design, XSA export, Vitis platform and overlay generation, and device-tree overlay preparation.

The PetaLinux project was configured and the build was initiated. However, the build encountered seven dependency-fetch failures, and successful completion of the full Linux build remained pending.

### 7. Scope of This Documentation

This repository organizes the technical architecture, tools, development workflow and build observations associated with the Kria KV260 SmartCam project.

It is intended as technical documentation and a learning reference, rather than a claim that every implementation stage was independently developed by the repository owner.
