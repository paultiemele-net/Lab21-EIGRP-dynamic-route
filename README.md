# Lab21-EIGRP-dynamic-route
This repository contains a Cisco lab that demonstrates EIGRP routing across multiple routers, enabling full connectivity between LANs through WAN links. The lab simulates a real-world enterprise network where traffic must traverse several routers to reach remote networks.

In this setup, four routers are connected via WAN subnets, and three LANs host PCs that communicate with each other. EIGRP dynamically exchanges routing information within AS 100, allowing seamless end-to-end communication without static routes.

Key Learning Objectives

Configure and operate EIGRP across multiple routers

Understand multi-router topology design and LAN-to-LAN routing

Set up DHCP pools on edge routers

Configure router IDs for deterministic routing

Validate routing with ICMP ping tests

Topology Overview

Routing Protocol: EIGRP (AS 100)

Routers: 4 Cisco routers (R1–R4)

LAN Networks:

PC1: 10.10.10.0/24

PC2: 40.40.40.0/24

PC3: 70.70.70.0/24

WAN Networks:

20.20.20.0/24

30.30.30.0/24

50.50.50.0/24

60.60.60.0/24

Traffic Flow

Traffic from PC1 traverses the network using EIGRP-learned routes to reach PC2 and PC3, allowing dynamic routing without manual static routes.

Validation

Check EIGRP neighbor adjacencies (show ip eigrp neighbors)

Review routing tables (show ip route)

Test connectivity with ICMP ping between all PCs
