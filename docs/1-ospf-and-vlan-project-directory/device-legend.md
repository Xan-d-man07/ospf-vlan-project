# Device Legend

Owner: Adeoluwa Dosunmu

Each Switch Is an Individual Network Comprised of VLANS.

| Device | Vlan | Network | Interfaces from  the connected Router | IP Address per PC |
| --- | --- | --- | --- | --- |
| Display Name- N1Switch  Hostname-Network_1_Switch | Hosts 10,20,30 | 1 |  |  |
| PC0 | 10 | 1 | Fa0/1 | 10.0.0.2 |
| PC1 | 10 | 1 | Fa0/2 | 10.0.0.3 |
| PC2 | 20 | 1 | Fa0/6 | 20.20.0.3 |
| PC3 | 20 | 1 | Fa0/5 | 20.20.0.2 |
| PC4 | 30 | 1 | Fa0/7 | 30.0.0.2 |
| PC5 | 30 | 1 | Fa0/8 | 30.0.0.3 |
|  |  |  |  |  |
| Display Name- N2Switch  Hostname-Network_2_Switch | Hosts 40,50 | 2 |  |  |
| PC8 | 40 | 2 | Fa0/4 | 40.40.0.2 |
| PC9 | 40 | 2 | Fa0/3 | 40.40.0.3 |
| PC10 | 50 | 2 | Fa0/6 | 50..50.50.3 |
| PC11 | 50 | 2 | Fa0/5 | 50..50.50.2 |
|  |  |  |  |  |
| Display Name- N3Switch  Hostname-Network_3_Switch | Hosts 60 | 3 |  |  |
| PC6 | 60 | 3 | Fa0/3 | 60.0.0.2 |
| PC7 | 60 | 3 | Fa0/4 | 60.0.0.3 |

| Switch | Network | IP Per VLAN | IP per Interface |
| --- | --- | --- | --- |
| Display Name- N1Switch  Hostname-Network_1_Switch | 1 | VLAN 10 - 10.0.0.10/8   VLAN 20- 20.20.0.10/16  VLAN 30-30.0.0.10/8 | Gig0/1 - 192.168.10.1 /24  Gig0/2-192.168.30.1 /24 |
|  |  |  |  |
| Display Name- N2Switch  Hostname-Network_2_Switch | 2 | VLAN 40- 40.40.0.10 /16 VLAN 50- 50.50.50.10/24 | Gig0/1 - 192.168.10.2 /24  Gig0/2-192.168.20.2/24 |
|  |  |  |  |
| Display Name- N3Switch  Hostname-Network_3_Switch | 3 | VLAN 60- 60.0.0.10/8  | Gig0/1 - 192.168.20.1 /24  Gig0/2-192.168.30.2 /24 |


--- 
[Back to Home](../../README.md)