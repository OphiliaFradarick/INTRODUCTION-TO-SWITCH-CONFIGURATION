# INTRODUCTION-TO-SWITCH-CONFIGURATION

# VLAN (Virtual LAN)
A group of host computers and servers that are configured as if they are in the same LAN, even if they reside across routers in separate LANs
The three types of VLAN are 
1. Port-based VLAN
2. Tag-based VLAN
3. Protocol-based VLAN

There are two approaches to assigning VLAN membership:
 ● Static VLAN: This is basically a port-based VLAN. The assignments are 
created when ports are assigned to a specific VLAN.
 ● Dynamic VLAN: Ports are assigned to a VLAN based on either the computer’s 
MAC address or the username of the client logged on to the computer. 
This means the system has been previously configured with the VLAN 
assignments for the computer or the username. The advantage of this is that 
the username and/or the computer can move to a different location, and 
VLAN membership is retained

Set layer 3 access to the switch by using the following command sequence:
 ● SwitchA(config)# interface VLAN 1
 ● SwitchA(config-if)# ip address 172.16.32.2 255.255.255.0
 ● SwitchA(config-if)#  no shutdown
 
![image](https://github.com/user-attachments/assets/08d7d5de-aa9c-4997-8d2a-98e2313dc9b2)

![image](https://github.com/user-attachments/assets/5fc78bd5-aacf-407d-8299-d9e850b1d4ac)

## VLAN TRUNKING
VLAN trunking is used to inter-connect the VLANs on a number of switches. 
A trunk is a point-to-point link between two network devices that carries packets from more than one VLAN. With VLAN trunking, you can extend your configured VLANs across the entire network. 
Most Cisco switches supports the IEEE 802.1Q protocol used to coordinate trunks on both FastEthernet and GigabitEthernet ports.

![image](https://github.com/user-attachments/assets/c6c3d025-374a-454c-88b1-9d63134ba67b)


