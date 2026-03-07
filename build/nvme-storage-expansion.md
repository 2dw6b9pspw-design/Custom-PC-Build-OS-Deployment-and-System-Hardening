# NVMe Boot Drive Migration and Storage Expansion

## Objective
Upgrade workstation storage and move the primary OS NVMe drive to the CPU-connected M.2 slot for better performance and cleaner lab separation.

## Environment
- Motherboard: ASUS TUF Gaming motherboard
- Primary Drive: Samsung 990 Pro with Heatsink 1TB
- Secondary Drive: WD Black SN850X 2TB
- OS: Windows 11

## Reason for Change
The original OS drive was not installed in the primary M.2 slot. The goal was to:
- Move the boot drive to M.2_1
- Install a second NVMe SSD for lab storage
- Keep the OS drive separated from lab workloads

## Procedure
1. Powered down the workstation and unplugged the system.
2. Opened the case and identified both M.2 slots.
3. Removed the Samsung 990 Pro from the lower M.2 slot.
4. Installed the Samsung 990 Pro into M.2_1 (top slot / CPU-connected lane).
5. Installed the WD Black SN850X 2TB into M.2_2.
6. Booted into BIOS and verified both NVMe drives were detected.
7. Confirmed Windows Boot Manager was still pointed to the Samsung 990 Pro.
8. Booted into Windows successfully.
9. Opened Disk Management.
10. Initialized the new SSD using GPT.
11. Created a new NTFS volume.
12. Renamed the new drive to LABS (D:).

## Validation
### BIOS Detection
- M.2_1: Samsung SSD 990 PRO with Heatsink 1TB
- M.2_2: WD Black SN850X 2TB
- Boot device: Windows Boot Manager on Samsung 990 Pro

### Windows Disk Management
- Disk 0: Samsung 990 Pro 1TB
- Disk 1: WD Black SN850X 2TB
- Partition style: GPT
- File system: NTFS

### Final Result
- C: Samsung 990 Pro 1TB for OS and applications
- D: LABS 2TB for labs, tools, VMs, and datasets

## Lessons Learned
- The primary NVMe slot should be used for the OS drive when possible.
- GPT is the correct partition style for modern UEFI Windows systems.
- Separating the OS drive from lab storage improves organization and scalability.
- BIOS verification and Windows disk provisioning should always be documented after hardware changes.

## Screenshots
Add the following screenshots to the images folder and link them here:
- Motherboard before SSD migration
- Motherboard after SSD migration
- BIOS showing both NVMe drives
- Disk initialization in Windows
- Final Disk Management layout
- Final File Explorer view showing C: and LABS (D:)
