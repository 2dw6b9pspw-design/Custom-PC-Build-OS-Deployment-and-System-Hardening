# Discrete GPU Installation and Verification

## Objective

Install and verify a discrete GPU on the workstation used to host the Monroe Redstone Technology Group (MRTG) IAM lab environment.

While the virtualized IAM infrastructure does not require GPU acceleration, a dedicated GPU improves host system responsiveness and ensures stable display output when managing multiple virtual machines.

---

## Hardware

**GPU Installed**

• MSI NVIDIA GeForce RTX 5060 Ti  

**Motherboard**

• ASUS TUF Gaming B650-PLUS WIFI

---

## Pre-Installation State

Prior to installation, the system relied on the CPU's integrated graphics.  
The primary PCIe x16 slot on the motherboard was unoccupied.

<p align="center">
<img src="../images/GPU_pre_install.png" width="650">
</p>

<p align="center">
Primary PCIe x16 slot prior to GPU installation.
</p>

---

## GPU Installation

The RTX 5060 Ti was installed into the motherboard's primary PCIe x16 slot and secured to the case.

<p align="center">
<img src="../images/GPU_post_install.png" width="650">
</p>

<p align="center">
RTX 5060 Ti installed in the primary PCIe x16 slot on the ASUS TUF motherboard.
</p>

---

## PCIe Power Connection

The GPU requires supplemental power from the power supply.  
After installing the card, the PCIe power cable was connected.

<p align="center">
<img src="../images/GPU_PCIe.png" width="650" style="transform: 
</p>

<p align="center">
PCIe power cable connected to the RTX 5060 Ti.
</p>
---

## Verification

After booting the system, Windows successfully detected the GPU.

Verification was performed using **Windows Device Manager**, confirming that both the integrated graphics and NVIDIA GPU were recognized by the operating system.

<p align="center">
<img src="../images/gpu-device-manager.png" width="650">
</p>

<p align="center">
Device Manager showing successful detection of the NVIDIA GeForce RTX 5060 Ti.
</p>

---

## Outcome

The workstation now includes a discrete GPU providing reliable graphical output and improved usability when managing multiple virtual machines.

The system is fully prepared to support the virtualization infrastructure used throughout the MRTG IAM lab series.
