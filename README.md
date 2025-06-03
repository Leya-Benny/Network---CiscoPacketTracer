Required Resources
Three (3) Multilayer Switches (Cisco Catalyst 1000 Series with Cisco IOS Release 15.1+ image)
Four (4) PCs (Windows with Terminal Emulation Program)
1 Laptop (Rogue)
Cables:
Console cables to configure the Cisco IOS devices via the console port.
Ethernet cables as shown in the topology.

Device
Interface
IP Address
Subnet Mask / CIDR
Default Gateway
SW1
VLAN88
192.168.88.2
255.255.255.0
N/A
SW2
VLAN88
192.168.88.3
255.255.255.0
N/A
SW3
VLAN88
192.168.88.4
255.255.255.0
N/A
PC0
NIC
192.168.15.15
255.255.255.0
192.168.15.1
Laptop0
NIC
192.168.25.25
255.255.255.0
192.168.25.1
PC1
NIC
192.168.15.16
255.255.255.0
192.168.15.1
Laptop1
NIC
192.168.25.26
255.255.255.0
192.168.25.1

Addressing Table

Lab Description
In this lab, you are required to troubleshoot all the connectivity issues. 

Instructions
Step 1: Setting Up the Network Topology
Simulate the topology by using all the devices mentioned above and then cable all the devices together:
Turn on the devices.
Connect the PCs with their respective switches.
Make sure all the lights between switches and PCs are active / green.
Step 2: Configure PCs
Configure the following on PCs according to the addressing table:
IP address
Subnet Mask
Default Gateway
Step 3: Configure and Verify
Configure and verify the following switch settings on each switch:
Console into the switch and enter the global configuration mode:
Assign the switch a name according to the addressing table.
Disable unwanted DNS lookup.
Configure SVI on each switch per the addressing table.
Enter a login MOTD banner to warn about illegal access.
Encrypt all current and future passwords.
Save the configuration.
Step 4: Configuration from Appendix
Switch
Ports
Assignment
Network
SW1
G1/0/1
802.1Q Trunk
N/A
G1/0/2-10
VLAN15
192.168.15.0/24
G1/0/11-18
VLAN25
192.168.25.0/24
SW2
G1/0/2
802.1Q Trunk
N/A
G1/0/2-10
VLAN15
192.168.15.0/24
G1/0/11-18
VLAN25
192.168.25.0/24
SW3
G1/0/1-2
802.1Q Trunk
N/A
G1/0/2-10
VLAN15
192.168.15.0/24
G1/0/11-18
VLAN25
192.168.25.0/24

Step 5: Troubleshoot VLAN 15 on SW1, SW2, and SW3
VLAN15 is supposed to be configured on all switches per the addressing table mentioned above.
Ping from PC0 to PC1
Step 6: Troubleshoot VLAN 25 on SW1, SW2, and SW3
VLAN25 is supposed to be configured on all switches per the addressing table mentioned above.
Ping from Laptop0 to Laptop1

