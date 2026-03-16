# Discrete GPU Installation and Verification

## Objective

Install and verify a discrete GPU on the workstation used to host the Monroe Redstone Technology Group (MRTG) IAM lab environment.

Although the IAM environment itself does not require GPU acceleration, a dedicated GPU improves host system responsiveness and provides stable display output while managing multiple virtual machines.

---

## Hardware

GPU Installed

• MSI NVIDIA GeForce RTX 5060 Ti

Motherboard

• ASUS TUF Gaming B650-PLUS WIFI

---

## Pre-Installation State

Prior to installation, the system relied on integrated graphics provided by the CPU.

![GPU Pre Install](images/GPU_pre_install.png)

---

## GPU Installation

The GPU was installed into the primary PCIe x16 slot on the motherboard.

![GPU Installed](images/GPU_post_install.png)

---

## PCIe Power Connection

The GPU requires supplemental PCIe power from the power supply.  
The power cable was connected after seating the card in the PCIe slot.

![PCIe Power Connection](images/GPU_PCIe.png)

---

## Verification

After booting the system, Windows successfully detected the GPU.

Verification was performed using Device Manager.

![Device Manager GPU Detection](images/gpu-device-manager.png)

Both the integrated graphics and the NVIDIA GPU are visible, confirming successful installation.

---

## Outcome

The workstation now includes a discrete GPU providing reliable display output and improved usability while managing multiple virtual machines for the MRTG IAM lab environment.
