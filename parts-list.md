# Parts List & Component Rationale

This document outlines the components selected for the system build and the rationale behind each decision, with an emphasis on performance, reliability, cost efficiency, and future upgrade potential.

# Workstation Parts List

This document lists the hardware components used in the workstation build.

---

## System Components Summary

| Component | Model |
|----------|------|
| CPU | AMD Ryzen 5 7600X3D |
| CPU Cooler | Thermalright Peerless Assassin 120 SE ARGB |
| Motherboard | ASUS TUF Gaming B650-PLUS WIFI (AM5) |
| Memory | Kingston Fury Beast 32GB (2x16GB) DDR5 6000 MT/s CL36 |
| GPU | MSI RTX 5060 Ti Gaming OC |
| Storage | Samsung 990 Pro 1TB NVMe PCIe 4.0 (Heatsink) |
| Storage | WD Black SN850X 2TB NVMe PCIe 4.0 |
| Power Supply | Corsair RM Series 1000W 80+ Gold (Fully Modular) |
| Case | NZXT H6 Flow RGB |

---

## Storage Configuration

| Drive | Model | Purpose |
|------|------|------|
| NVMe 1 | Samsung 990 Pro 1TB | Operating System / Applications |
| NVMe 2 | WD Black SN850X 2TB | Lab environments / Virtual Machines |

---

## Notes

- The Samsung 990 Pro is installed in the **primary CPU-connected M.2 slot**.
- The WD Black SN850X is installed in the **secondary chipset-connected M.2 slot**.
- Storage separation allows lab workloads and virtual machines to run independently of the operating system.


## Component Selection & Rationale

### CPU: AMD Ryzen 5 7600X3D
Selected as part of a Micro Center bundle that provided the best performance-to-cost ratio among available options. Higher-tier Ryzen 7 and Ryzen 9 CPUs were evaluated but were not justified for the intended gaming-focused workload.

The Ryzen 5 7600X3D features AMD’s 3D V-Cache technology with 96MB of L3 cache, significantly improving gaming performance by reducing memory latency. This CPU provides strong current performance while remaining efficient and suitable for future upgrades.

---

### CPU Cooler: Thermalright Peerless Assassin 120 SE ARGB
Chosen for its strong thermal performance at a competitive price point. This dual-tower air cooler provides cooling capacity comparable to more expensive solutions while avoiding the complexity and maintenance considerations of liquid cooling.

The cooler delivers quiet operation under load, sufficient thermal headroom for the selected CPU, and AM5 compatibility. ARGB lighting was included without added cost and integrates with the system’s overall aesthetic.

---

### Motherboard: ASUS TUF Gaming B850-PLUS WiFi (AM5)
Selected to complement the CPU and provide long-term expandability. Key features include:

- Support for up to 256GB DDR5 memory  
- PCIe 5.0 support  
- Three M.2 NVMe slots  
- 2.5Gb Ethernet and WiFi 7  
- USB Type-C connectivity  

The ASUS TUF lineup uses reinforced components designed for durability and reliability, making it well-suited for sustained use and future hardware upgrades.

---

### Memory: Kingston Fury Beast 32GB (2x16GB) DDR5 6000 MT/s CL36
Selected for optimal compatibility with the AM5 platform and Ryzen memory performance recommendations. This kit provides sufficient capacity for modern gaming and general-purpose workloads.

RGB memory was considered but ultimately unnecessary due to cooler clearance and lack of functional benefit. The non-RGB kit provided significant cost savings while maintaining performance.

---

### GPU: MSI RTX 5060 Ti Gaming OC

A discrete GPU was installed to provide reliable display performance and improve overall system responsiveness when managing multiple virtual machines.

While the IAM lab environment itself does not rely on GPU acceleration, a dedicated GPU ensures stable video output and prevents the CPU from handling graphical workloads while running virtualization tasks.

Key considerations included:

• Reliable display output during virtualization workloads  
• Reduced graphical load on the CPU while managing multiple VMs  
• Potential future support for GPU-accelerated development workloads

The GPU does not directly impact the identity infrastructure but improves the overall usability and stability of the workstation hosting the lab environment.

---

### Storage: Samsung 990 Pro 1TB NVMe PCIe 4.0
Chosen to balance performance, capacity, and cost. After evaluating 500GB and 2TB options, 1TB was selected as the most practical capacity for the intended workload.

The Samsung 990 Pro offers excellent sequential and random performance, strong reliability, and integrated heatsink cooling. PCIe 5.0 storage was evaluated but excluded due to minimal real-world benefit at a significantly higher cost.

---

### Power Supply: Corsair RMe Series 1000W 80+ Gold (Fully Modular)
The first component purchased for this build. While 1000W exceeds current system requirements, it provides ample headroom for future upgrades and ensures stable power delivery.

The fully modular design simplifies cable management, improves airflow, and supports long-term system scalability.

---

### Case: NZXT H6 Flow RGB
Selected for its airflow-focused dual-chamber design and clean aesthetic. Key features include:

- Wraparound tempered glass panels for component visibility  
- Dual-chamber layout for improved thermals and cable management  
- Three pre-installed 120mm RGB fans  
- Support for radiators up to 360mm  
- Tool-free panel access for maintenance and upgrades  

This case balances cooling performance, ease of assembly, and visual appeal.

---

## Summary

All components were selected to meet current performance needs while allowing for future expansion and upgrades. Emphasis was placed on reliability, compatibility, and cost-effective performance rather than unnecessary overprovisioning.
