# Cisco Business Network with VLAN Segmentation & Internet Connectivity

## Project Overview

This project is a simulated business network designed and configured in **Cisco Packet Tracer**. The network simulates how a small business can use VLAN segmentation, inter-VLAN routing, DHCP, NAT/PAT, and Internet based network services to create a structured and functional network environment.

## Network Topology

                         Simulated Internet
                                |
                         [Internet Server]
                     198.51.100.10 /24
                                |
                         [ISP Router]
                                |
                         [Business Router]
                                |
                             [Switch]
                       /        |        \
                  VLAN 10   VLAN 20   VLAN 30
                    |          |          |
                 Devices    Devices    Devices

## Technologies & Concepts
* VLANs
* Inter-VLAN Routing
* Router on a Stick
* DHCP
* IPv4 Addressing
* Subnetting
* Default Routing
* NAT/PAT
* WAN Connectivity
* DNS
* NTP
* HTTP/HTTPS
* FTP
* Email Services
* Network Troubleshooting

## VLAN Structure

| VLAN    | Network         | Default Gateway |
| ------- | --------------- | --------------- |
| VLAN 10 | 192.168.1.0/24 | 192.168.1.1    |
| VLAN 20 | 192.168.2.0/24 | 192.168.2.1    |
| VLAN 30 | 192.168.3.0/24 | 192.168.3.1    |

Each VLAN represents a separate department within the business network.

## What I Configured

### 1. VLAN Segmentation

Created three separate VLANs on the switch to separate devices into different departments.

### 2. Inter-VLAN Routing

Configured router on a stick using router sub interfaces to allow devices in different VLANs to communicate when permitted.

### 3. DHCP

Configured DHCP pools on the office router to automatically assign IP addresses to devices within each VLAN.

DHCP provided:

* IP addresses
* Subnet masks
* Default gateways
* DNS server information

Reserved gateway and other infrastructure addresses using DHCP excluded-address commands.

### 4. WAN Connectivity

Connected the business router to an ISP router using a dedicated point to point WAN network.

### 5. NAT/PAT

Configured NAT overload to allow multiple internal devices to share the business router's external/WAN address when accessing the simulated Internet.

### 6. Internet Services

Configured a simulated Internet server with several network services:

* DNS
* HTTP
* HTTPS
* FTP
* Email
* NTP

### 7. Connectivity Testing & Troubleshooting

Tested connectivity throughout the network using tools such as:

ping, 
show ip interface brief, 
show ip route, 
show ip nat translations, 
show access-lists

## Key Learning Outcomes

Through this project, I gained practical experience with:

* Designing a structured business LAN
* Creating and managing multiple VLANs
* Configuring inter-VLAN routing
* Implementing DHCP across multiple networks
* Configuring WAN connectivity
* Understanding default routes
* Implementing NAT/PAT
* Deploying basic network services
* Troubleshooting connectivity issues
* Verifying network configurations using Cisco IOS commands

## Project Goal

The main goal of this project was to build a more complete business network that combines **LAN segmentation, routing, automated addressing, WAN connectivity, NAT, and simulated network services**.

