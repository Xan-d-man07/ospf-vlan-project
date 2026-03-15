# Network 1 Setup

Owner: Adeoluwa Dosunmu

Renaming Switch

`Switch>enable
Switch#configure terminal
Switch(config)#hostname Network_1_Switch`

Initializing VLANS for Network 1

- configure terminal
- vlan 10
- name v1
- vlan 20
- name v2
- vlan 30
- name v3

Enable routing for the Switch

`Network_1_Switch(config)#ip routing`

Assigning interfaces to VLANS

```jsx
Network_1_Switch# configure  terminal
Network_1_Switch(config)#interface range fa0/1-2
Network_1_Switch(config-if-range)#switchport access vlan 10

Network_1_Switchconfig-if-range)#interface range fa0/5-6
Network_1_Switch(config-if-range)#switchport access vlan 20

Network_1_Switch(config-if-range)#inteerface range fa0/7-8
Network_1_Switch(config-if-range)#switchport access vlan 30
Network_1_Switch(config-if-range)#end
```

Assigning IP’s to the Switches for the VLANS

```jsx
N1Switch(config)#interface vlan 10
N1Switch(config-if)#ip address 10.0.0.10 255.0.0.0

N1Switch(config-if)#interface vlan 20
N1Switch(config-if)#ip address 20.20.0.10 255.255.0.0

N1Switch(config-if)#interface vlan 30
N1Switch(config-if)#ip address 30.0.0.10 255.0.0.0
```
---

- [Previous Page](2-0creating-networks-and-set-up-vlans-directory.md)
- [Next Page](2-2-network-2-setup.md)
- [Back to Home](../../README.md)