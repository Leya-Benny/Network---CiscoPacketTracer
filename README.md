# 🔧 Network Troubleshooting Lab – VLAN & Switch Configuration

## 📚 Lab Description
This lab simulates a small network using multilayer switches, PCs, and laptops to practice VLAN setup and troubleshoot connectivity issues across VLANs 15 and 25.

---

## 🧰 Required Resources

- **Multilayer Switches:** 3x Cisco Catalyst 1000 Series (Cisco IOS Release 15.1+)
- **PCs:** 4x Windows PCs with Terminal Emulation Program
- **Laptop:** 1x Rogue Laptop (simulates rogue activity)
- **Cabling:**
  - Console cables (for IOS configuration)
  - Ethernet cables (as per topology)

---

## 🗂 Addressing Table

| Device   | Interface | IP Address     | Subnet Mask       | Default Gateway |
|----------|-----------|----------------|-------------------|-----------------|
| SW1      | VLAN88    | 192.168.88.2   | 255.255.255.0     | N/A             |
| SW2      | VLAN88    | 192.168.88.3   | 255.255.255.0     | N/A             |
| SW3      | VLAN88    | 192.168.88.4   | 255.255.255.0     | N/A             |
| PC0      | NIC       | 192.168.15.15  | 255.255.255.0     | 192.168.15.1    |
| PC1      | NIC       | 192.168.15.16  | 255.255.255.0     | 192.168.15.1    |
| Laptop0  | NIC       | 192.168.25.25  | 255.255.255.0     | 192.168.25.1    |
| Laptop1  | NIC       | 192.168.25.26  | 255.255.255.0     | 192.168.25.1    |

---

## 🛠️ Instructions

### ✅ Step 1: Set Up the Network Topology
- Power on all switches, PCs, and laptops.
- Connect each PC and laptop to the appropriate switch ports.
- Ensure Ethernet link lights are **active (green)**.

### ✅ Step 2: Configure PCs & Laptops
On each PC/laptop:
- Assign the **IP address**, **subnet mask**, and **default gateway** as per the table above.

### ✅ Step 3: Configure Switches
On **SW1, SW2, and SW3**:
1. Console into the switch.
2. Enter global config mode.
3. Assign a hostname (SW1, SW2, SW3).
4. Disable DNS lookup:
   ```plaintext
   no ip domain-lookup


