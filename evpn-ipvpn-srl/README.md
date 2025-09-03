# EVPN-IPVPN interworking on SRL

This DCI lab shows EVPN-VXLAN and IPVPN-MPLS interworking on 7250 IXR-X1b running SR Linux.

## Topology
![image](srl-evpn-ipvpn-v2.jpg)

Client1 and Client2 on either DCs are connected over this infrastructure.

## Underlay
BGP is used as underlay protocol.
Leafs and Spines establish BGP sessions using IPv6 LLA.

## Overlay
All leaves establish BGP session with their DCGW and advertise EVPN address family.

## EVPN-IPVPN

On DCGW, a separate IP-VPN instance is created for each EVPN service.



