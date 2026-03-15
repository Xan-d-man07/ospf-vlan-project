# Network 2 setup

Owner: Adeoluwa Dosunmu

Rename Switch

```jsx
Switch>enable
Switch#configure terminal
Switch(config)#hostname Network_2_Switch
```

Enable routing for the Switch

`Network_1_Switch(config)#ip routing`

Setup VLANS

```jsx
Network_2_Switch(config)#vlan 40
Network_2_Switch(config-vlan)#name v4
Network_2_Switch(config-vlan)#vlan 50
Network_2_Switch(config-vlan)#name v5
Network_2_Switch(config-vlan)#exit
```

Assign Interfaces to VLANS

```jsx
Network_2_Switch(config)#interface range fa0/5-6
Network_2_Switch(config-if-range)#switchport access vlan 50
Network_2_Switch(config-if-range)#interface range fa0/3-4
Network_2_Switch(config-if-range)#switchport access vlan 40
```

Assign IP addresses to VLANS

```jsx
Network_2_Switch(config-if-range)#interface vlan 40
Network_2_Switch(config-if)#ip address 40.40.0.10 255.255.0.0
Network_2_Switch(config-if)#interface vlan 50
Network_2_Switch(config-if)#ip address 50.50.50.10 255.255.255.0
Network_2_Switch(config-if)#exit
Network_2_Switch(config)#end
```

Verify changes

`Network_2_Switch#show vlan brief`

---

- [Previous Page](2-1-network-1-setup.md)
- [Next Page](2-3-network-3-setup.md)
- [Back to Home](../../README.md)