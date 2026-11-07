# Embedded Linux and PetaLinux Workflow

## 1. Overview

The embedded Linux workflow prepares the software environment for the AMD Kria KV260 SmartCam platform.

PetaLinux provides the tools required to configure and build an embedded Linux system for the target hardware.

The reference workflow uses PetaLinux 2022.1 and the Yocto Project build system.

## 2. PetaLinux Environment

The development environment described in the reference material includes:

- PetaLinux 2022.1
- Ubuntu 18.04.6 LTS
- AMD Kria KV260 BSP
- Yocto Project
- BitBake

The KV260 board support package (BSP) provides a starting point for configuring the embedded Linux project.

## 3. Yocto and BitBake

The Yocto Project provides the framework for building customized embedded Linux distributions.

BitBake is the build engine used to process recipes, resolve dependencies and generate the required software components.

The workflow includes:
1. Initializing the PetaLinux project.
2. Configuring the target hardware.
3. Setting up the required build environment.
4. Processing recipes and dependencies through BitBake.
5. Building the embedded Linux image.

## 4. Device Tree Generation

The device tree describes the hardware components and their configuration to the Linux kernel.

The reference workflow uses XSCT and HSI to extract hardware information and generate device-tree source files.

The process includes:

1. Using the exported hardware platform as input.
2. Extracting hardware information.
3. Generating device-tree source files such as `.dtsi`.
4. Compiling the device-tree source using the Device Tree Compiler (DTC).
5. Generating device-tree overlay files (`.dtbo`) where required.

## 5. FPGA Manager and Overlay Integration

The embedded Linux workflow includes FPGA Manager-related integration.

The reference material describes the use of the `fpgamanager` recipe and `dfx-mgr` for FPGA configuration and management.

The acceleration overlay includes hardware configuration and metadata files such as:

- `bit.bin`
- `shell.json`

## 6. Build Process and Status

The PetaLinux build was initiated using the configured project environment.

However, the build did not complete successfully.

The reference report records seven `do_fetch` task failures involving dependencies such as:

- pkg-config
- bzip2
- OpenSSL
- Binutils
- GNU Config
- Pseudo
- glibc

The build stopped during the dependency-fetch stage. The exact root cause was not confirmed in the reference material.

Therefore, a successful final Linux image build and on-board SmartCam deployment are not claimed here.

## 7. Workflow Summary

The embedded Linux workflow can be represented as:

1. Import the KV260 hardware platform.
2. Configure the PetaLinux project using the board support package.
3. Generate the device tree.
4. Integrate FPGA Manager and acceleration overlay support.
5. Resolve build dependencies.
6. Build the embedded Linux image.
7. Prepare the image and hardware artifacts for target-board deployment.

## 8. Project Scope and Attribution

This document summarizes the embedded Linux workflow and build status described in the technical reference material.

The documented build failure is retained for technical accuracy. This repository does not claim a successful Linux image build or complete on-board deployment.
