# Project Description
This project demonstrates InterVLAN routing and OSPF configuration across multiple networks using Cisco Packet Tracer. It is designed to showcase VLAN segmentation, Layer 3 switching, and dynamic routing in a hands-on environment.

## Details
- Create multiple VLANs across three networks
- Configure InterVLAN routing using Layer 3 switches
- Establish OSPF routing between networks
- Verify connectivity and routing tables


## 🌐 Network Topology
- All Networks are connected using OSPF Configuration
- All networks in Area 0
- Proper route advertisement verified via show ip route

Network 1
---
- VLANs: 10, 20, 30
- Layer 3 switch for InterVLAN routing
- Minimum 2 hosts per VLAN

Network 2
---
- VLANs: 40, 50
- InterVLAN routing
- Minimum 2 hosts per VLAN

Network 3
---
- VLAN: 60
- InterVLAN routing
- Minimum 2 hosts





## Diagrams
- [Topology- Hand-drawn](Diagrams/topology.png)
- [Finished Layout](Diagrams/ospf-vlan_finished_layout.png)



## Documentation (These are steps and should be followed one after the other for ease of understanding)
- [Ospf And Vlan Project Directory ](docs/1-ospf-and-vlan-project-directory/1-1-directory.md)
- [Creating Networks And Set Up Vlans ](docs/2-creating-networks-and-setup-vlans/2-0creating-networks-and-set-up-vlans-directory.md)
- [Ospf Configuration ](docs/3-ospf-configuration/3-0-ospf-configuration-directory.md)
- [Save Configurations ](docs/4-save-configurations.md)
- [Packet Tracer file](Packet-Tracer-file/ospf-and-vlan-project-completed.pkt)
- [Proof of Connectivity](proof_of_connectivity/0-proof-directory.md)

