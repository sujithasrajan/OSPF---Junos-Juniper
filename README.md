# OSPF---Junos-Juniper

We have set up a network consisting of 4 routers running OSPF as shown in the figure.


1. Allocated IP addresses and networks from the address block and assigned them to the router's interfaces for both physical and loopback interfaces.

2. Configured the interfaces according to the IP address assignment. We can verify the physical connectivity and the correctness of the interface configuration by pinging the connected interfaces of the remote routers from the local router.

3. Add the physical and loopback interfaces to the firewall’s trust zone to allow for inbound ping and traceroute commands as well as OSPF protocol.

4. Configured OSPF on this multi-area network using the IP addresses of the loopback interfaces as OSPF router IDs. 

5. Added the loopback interfaces to OSPF as passive interfaces to prevent them from forming adjacencies. Verify that all routers learn routes from each other via OSPF by checking that all networks configured on all the remote router's loopback interfaces show up in
the local router’s routing table.

6. We can Verify that all routers are reachable from all other routers by pinging every remote router’s loopback interface from the local router.

![FLOW/STATE DIAGRAM](https://github.com/sujithasrajan/OSPF-Junos-Juniper/blob/master/OSPF/OSPF-PyEZ/OSPF_Topology.png)

