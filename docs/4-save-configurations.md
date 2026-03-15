# Save Configurations

Owner: Adeoluwa Dosunmu

This makes sure that your changes are saved permanently, so every time you boot up the file it reloads from that saved states, so you don’t loose any progress 

Network 1

```jsx
Network_1_Switch#copy running-config startup-config
Destination filename [startup-config]? 
Building configuration...
[OK]
Network_1_Switch#
```

Network 2

```jsx
Network_2_Switch>
Network_2_Switch>enable
Network_2_Switch#copy running-config startup-config
Destination filename [startup-config]? 
Building configuration...
[OK]
Network_2_Switch#
```

Network 3

```jsx
Network_3_Switch>
Network_3_Switch>enable
Network_3_Switch#copy running-config startup-config
Destination filename [startup-config]? 
Building configuration...
[OK]
Network_3_Switch#
```

---

- [Previous Page](../docs/3-ospf-configuration/3-2-ospf-on-routers.md)
- [Proof](../proof_of_connectivity/0-proof-directory.md)
- [Back to Home](../README.md)