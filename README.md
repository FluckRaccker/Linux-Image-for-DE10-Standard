# Linux Image for DE10-Standard (Cyclone V SoC)

![Platform](https://img.shields.io/badge/Platform-DE10--Standard-blue)
![SoC](https://img.shields.io/badge/SoC-Cyclone%20V-orange)
![OS](https://img.shields.io/badge/Linux-Debian-green)
![Python](https://img.shields.io/badge/Python-3.x-yellow)

Prebuilt Linux image for the **Terasic DE10-Standard FPGA board** with **Python support** enabled.

This image was created to simplify development using the **HPS (ARM Cortex-A9)** of the Cyclone V SoC, allowing quick access to Python for communication with FPGA peripherals.

The goal is to provide an easy way to start **HPS–FPGA development** without having to build a full Linux system.

---

# Table of Contents

- [Overview](#overview)
- [Download](#download)
- [Features](#features)
- [Hardware Requirements](#hardware-requirements)
- [Flashing the SD Card](#flashing-the-sd-card)
- [Booting the Board](#booting-the-board)
- [Default Login](#default-login)
- [Testing Python](#testing-python)
- [Accessing FPGA from HPS](#accessing-fpga-from-hps)
- [Typical Applications](#typical-applications)
- [Boot Files Structure](#boot-files-structure)
- [Contributing](#contributing)
- [License](#license)
- [Author](#author)

---

# Overview

The **DE10-Standard** board integrates:

- ARM Cortex-A9 HPS
- Cyclone V FPGA fabric
- HPS–FPGA AXI bridges

Running Linux on the HPS enables powerful applications such as:

- FPGA control using Python
- Real-time signal processing
- Embedded system prototyping
- Data acquisition systems

This repository provides a **ready-to-use Linux image** to accelerate development.

---

# Download

The Linux image is available at:

**Google Drive**

https://drive.google.com/drive/folders/1Wi2vJvuFiaZFCItfh3o6dweIzVawJOvK?usp=sharing

Files included:
