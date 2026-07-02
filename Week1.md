Campus Architecture and Design Principles:

**Heirarchy**
1- what is the overall hierarchical structure of the campus and what features and functions should be implemented at each layer of the hierarchy?
2- what are the key modules or building blocks and how do they relate to each other and work in the overall hierarchy? 


Traditional 3 tier architecture components:

********Access Layer*******
The access layer provides the intelligent demarcation between the network infrastructure and the computing devices that leverage that infrastructure. As such it provides a security, QoS, and policy trust boundary. It is the first layer of defense in the network security architecture and the first point of negotiation between end devices and the network infrastructure.

**Table 1 Examples of Types of Service and Capabilities**

###############Service Requirements                =========> Service Features###############

Discovery and Configuration Services ========> 802.1AF, CDP, LLDP, LLDP-MED

Security Services                    ========>  IBNS (802.1X), (CISF): port security, DHCP snooping, DAI, IPSG

Network Identity and Access          ========>  802.1X, MAB, Web-Auth

Application Recognition Services     ========>   QoS marking, policing, queuing, deep packet inspection NBAR, etc.

Intelligent Network Control Services =========>  PVST+, Rapid PVST+, EIGRP, OSPF, DTP, PAgP/LACP, UDLD, FlexLink, Portfast, UplinkFast, BackboneFast, LoopGuard, BPDUGuard, Port Security, RootGuard

Physical Infrastructure Services     =========>  Power over Ethernet


*******Distribution*******

The aggregation point. Access layer switches uplink directly to this layer. This is where the boundary between Layer 2 (switching) and Layer 3 (routing) traditionally sits. It handles policy control, routing boundaries, access control lists (ACLs), and queuing.


*******Core*********

The high-speed backbone. The core’s sole purpose is to move traffic between different distribution blocks as fast as humanly possible. Architectural Rule: Never let security filtering, policy enforcement, or user packets terminate directly on the core. It must remain lean and lightning-fast.





