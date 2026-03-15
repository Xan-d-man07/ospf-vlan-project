# Setup Interfaces

Owner: Adeoluwa Dosunmu

- Make sure outward interfaces i.e. GigabitEthernet 0/1 and 0/2 are not switchports
- Assign IP to outward interfaces
- Repeat for other interface

```jsx
Network_1_Switch(config)#interface GigabitEthernet0/1
Network_1_Switch(config-if)#no switchport
Network_1_Switch(config-if)#ip address 192.168.10.2 255.255.255.0
Network_1_Switch(config-if)#interface GigabitEthernet0/2
Network_1_Switch(config-if)#no switchport
Network_1_Switch(config-if)#interface GigabitEthernet0/2
```

Repeat for all other Switches

```jsx
Network_2_Switch(config)#int gi0/1
Network_2_Switch(config-if)#no switchport
Network_2_Switch(config-if)#ip address 192.168.10.2 255.255.255.0
Network_2_Switch(config-if)#int gi 0/2
Network_2_Switch(config-if)#no switchport
Network_2_Switch(config-if)#ip address 192.168.20.2 255.255.255.0
```

```jsx
Network_3_Switch(config)#interface range GigabitEthernet 0/1-2
Network_3_Switch(config-if-range)#no shutdown
Network_3_Switch(config-if-range)#no switchport
Network_3_Switch(config-if-range)#exit
Network_3_Switch(config)#int gi0/1
Network_3_Switch(config-if)#ip address 192.168.20.1 255.255.255.0
Network_3_Switch(config-if)#int gi0/2
Network_3_Switch(config-if)#ip address 192.168.30.2 255.255.255.0
```
---

- [Previous Page](3-0-ospf-configuration-directory.md)
- [Next Page](3-2-ospf-on-routers.md)
- [Back to Home](../../README.md)