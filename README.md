# Linux Image for DE10-Standard (Cyclone V SoC)

Linux image for the **Terasic DE10-Standard FPGA board** with Python support, ready to run from an SD card.

This image was prepared to simplify development using the HPS (ARM Cortex-A9) of the Cyclone V SoC, allowing quick access to tools such as Python for communication with FPGA peripherals.


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
  - zImage
  - socfpga_cyclone5_socdk.dtb
  - extlinux folder
  - Linux root filesystem
  - Boot files


---

# Features

- Debian-based Linux system
- Python 3 installed
- Compatible with **Cyclone V SoC**
- Ready for **DE10-Standard**
- Access to HPS peripherals
- Suitable for FPGA interaction

--- 

# Flashing the Image to SD Card

## Linux / MacOS

Insert the SD card and identify the device:

```
lsblk
```

Write the image:

```
sudo dd if=de10_linux.img of=/dev/sdX bs=4M status=progress
sync
```

Replace:

```
/dev/sdX
```
with your SD card device.

## Windows

Use **Balena** Etcher or **Win32DiskImager**.

Steps:

1. Insert SD card
2. Open Balena Etcher
3. Select the image
4. Select the SD card
5. Flash

--- 

# Booting the Board

1. Insert the SD card into the DE10-Standard
2. Set the board to SD boot mode
3. Connect the USB-UART cable
4. Turn On the PuTTY serial console
5. Power on the board

The system should boot automatically.

## Default Login

```
user: root
password: root
```

## Connecting with PuTTY

You can access the Linux terminal through the serial console using PuTTY.

Download PuTTY:
https://www.putty.org/

### Serial configuration

Typical settings:

```
Connection type: Serial
Serial line: COMx
Speed (baud): 115200
```

After opening the connection, power on the board and the Linux boot messages should appear.

--- 

# Folder Structure

Example structure of the boot partition:


```
boot/
 ├── zImage
 ├── socfpga_cyclone5_socdk.dtb
 └── extlinux/
      └── extlinux.conf
```
--- 

# Author

**Rafael Luiz Ferreira** 

Federal University of Santa Catarina (UFSC)

Electronics Engineering

--- 

# Contributing

Contributions and improvements are welcome.

Feel free to open issues or pull requests.
