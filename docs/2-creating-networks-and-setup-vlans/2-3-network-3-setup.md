# Network 3 setup

Owner: Adeoluwa Dosunmu

Rename Switch

```jsx
Switch>enable
Switch#configure terminal
Switch(config)#hostname Network_3_Switch
```

Enable routing for the Switch

`Network_1_Switch(config)#ip routing`

Setup VLAN

```jsx
Network_3_Switch(config)#vlan 60
Network_3_Switch(config-vlan)#name v6
```

Assign interfaces to VLAN

```jsx
Network_3_Switch(config-vlan)#interface range fa0/3-4
Network_3_Switch(config-if-range)#switchport access vlan 60
Network_3_Switch(config-if-range)#interface vlan 60
```

Assign IP to VLAN

```jsx
Network_3_Switch(config-if)#ip address 60.0.0.10 255.0.0.0
Network_3_Switch(config-if)#end
```

Verify Changes
`Network_3_Switch#show vlan brief`


---
- [Previous Page](2-2-network-2-setup.md)
- [Next Page](../3-ospf-configuration/3-0-ospf-configuration-directory.md)
- [Back to Home](../../README.md)