# OSPF on Routers

Owner: Adeoluwa Dosunmu

- Note Adding Router id’s to each switch/router is optional.

Set up OSPF on Switch 1

```jsx
Network_1_Switch(config)#router ospf 1
Network_1_Switch(config-router)#router-id 1.1.1.1

Network_1_Switch(config-router)#network 192.168.10.0 0.0.0.255 area 0
Network_1_Switch(config-router)#network 192.168.20.0 0.0.0.255 area 0
Network_1_Switch(config-router)#network 192.168.30.0 0.0.0.255 area 0
	
Network_1_Switch(config-router)#network 10.0.0.0 0.255.255.255 area 0
Network_1_Switch(config-router)#network 20.20.0.0 0.0.255.255 area 0
Network_1_Switch(config-router)#network 30.0.0.0 0.255.255.255 area 0
Network_1_Switch(config-router)#network 40.40.0.0 0.0.255.255 area 0
Network_1_Switch(config-router)#network 50.50.50.0 0.0.0.255 area 0
Network_1_Switch(config-router)#network 60.0.0.0 0.255.255.255 area 0
```

setup OSPF on Switch 2

- Notice for this one I used subnet Summarization since the IP’s I used for the Switches as shown in the diagram follow    - - - 192.168.x.x 0.0.0.255 format
- So I changed it to 192.168.0.0 0.0.255.255 to catch them all, for convenience

```jsx
Network_2_Switch(config)#no router ospf 1
Network_2_Switch(config)#router ospf 1
Network_2_Switch(config-router)#router-id 2.2.2.2
Network_2_Switch(config-router)#network 192.168.0.0 0.0.255.255 area 0
Network_2_Switch(config-router)#network 10.0.0.0 0.255.255.255 area 0
Network_2_Switch(config-router)#network 20.20.0.0 0.0.255.255 area 0
Network_2_Switch(config-router)#network 30.0.0.0 0.255.255.255 area 0
Network_2_Switch(config-router)#network 40.40.0.0 0.0.255.255 area 0
Network_2_Switch(config-router)#network 50.50.50.0 0.0.0.255 area 0
Network_2_Switch(config-router)#network 60.0.0.0 0.255.255.255 area 0
```

setup OSPF on Switch 3

```jsx
Network_3_Switch(config)#router ospf 1
Network_3_Switch(config-router)#router-id 3.3.3.3
Network_3_Switch(config-router)#network 192.168.0.0 0.0.255.255 area 0
Network_3_Switch(config-router)#network 10.0.0.0 0.255.255.255 area 0
Network_3_Switch(config-router)#network 20.20.0.0 0.0.255.255 area 0
Network_3_Switch(config-router)#network 30.0.0.0 0.255.255.255 area 0
Network_3_Switch(config-router)#network 40.40.0.0 0.0.255.255 area 0
Network_3_Switch(config-router)#network 50.50.50.0 0.0.0.255 area 0
Network_3_Switch(config-router)#network 60.0.0.0 0.255.255.255 area 0
```
--- 

- [Previous Page](3-1-setup-interfaces.md)
- [Next Page](../4-save-configurations.md)
- [Back to Home](../../README.md)