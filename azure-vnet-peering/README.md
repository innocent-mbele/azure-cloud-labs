# Azure VNet Peering

## Overview

This project demonstrates how to connect two Azure Virtual Networks using Azure VNet Peering. The peering enables private communication between resources in different VNets over the Microsoft backbone network without using the public Internet.

### Virtual Networks

| Virtual Network | Address Space |
|-----------------|---------------|
| vnet-cloud-labs-dev-001 | 10.0.0.0/16 |
| vnet-uaenorth-1 | 172.16.0.0/16 |

### Configuration

- Created two Azure Virtual Networks
- Configured bidirectional VNet Peering
- Enabled virtual network access
- Verified peering status as **Connected** and **Fully Synchronized**

## Screenshots

- vnet-peering-01-connected.png
- vnet-peering-02-connected.png