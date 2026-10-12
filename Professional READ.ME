# CMPG 325 Individual Semester Project

**Kalahari Biodiversity Research Centre (Upington)**

| | |
|---|---|
| Student | Nyembezi, T (40183955) |
| Project ID | CMPG325-2026-107 |
| Client ID | CLI-107 |
| Industry | Research |
| Assigned addressing block | 192.168.48.0/24 |
| Assigned networking challenge | DNS (internal name resolution service) |
| Design constraint | No network downtime tolerated during month-end processing |
| Change request | CR11: Management adopts VoIP handsets, so voice traffic must be accommodated on the existing design |

## Project Overview

This project designs and simulates a network for the Kalahari Biodiversity Research Centre in Cisco Packet Tracer. The network supports administrative work (including month-end processing) and research work, provides internal name resolution (DNS), and accommodates VoIP handsets under change request CR11.

## Network Design Summary

The assigned block 192.168.48.0/24 is split into four equal /26 subnets, one per VLAN. Equal subnets were chosen for simplicity, because the assigned challenge is DNS rather than address-efficiency.

| VLAN | Department | Subnet | Gateway |
|------|------------|--------|---------|
| 10 | Admin | 192.168.48.0/26 | 192.168.48.1 |
| 20 | Research | 192.168.48.64/26 | 192.168.48.65 |
| 30 | Servers | 192.168.48.128/26 | 192.168.48.129 |
| 40 | Voice | 192.168.48.192/26 | 192.168.48.193 |

**Devices:** 1 router (2911, router-on-a-stick), 3 switches (2960: core, Admin, Research), 1 server (DNS and DHCP), 6 PCs, 2 IP phones.

**Key configuration:**

- VLANs on all switches, with access ports for end devices and trunk ports between switches and to the router
- Router sub-interfaces (Gi0/0.10, .20, .30, .40) for inter-VLAN routing
- DHCP pools for each VLAN on the server, with `ip helper-address` relay on the router
- Voice VLAN (40) on the phone ports, with phones powered by power adapter modules

## Assigned Challenge: DNS

The server (192.168.48.130) runs the DNS service, and DHCP hands the server's address to every client as its DNS server. The record `server.kbrc.local` resolves to 192.168.48.130.

**Verification:** `ping server.kbrc.local` from a PC in the Admin VLAN and from a PC in the Research VLAN resolves the name and gets replies (0% loss).

## Change Request CR11 (VoIP)

Voice traffic is carried on its own VLAN (40) with its own DHCP pool. Both phones received addresses (192.168.48.194 and 192.168.48.195) and are reachable from the router.

## Month-End Downtime Constraint

See the downtime constraint document in this repository. VLAN separation keeps faults inside one department. The document also states the design's limitations and the improvements recommended for production.

## Testing Summary

- All PCs receive correct addresses by DHCP
- DNS resolves from both the Admin and Research VLANs
- Cross-VLAN connectivity works (Research to Admin)
- Both phones receive Voice VLAN addresses and are reachable

## Troubleshooting Notes

- **DHCP failed at first (APIPA address):** `show interfaces trunk` showed that only VLANs 1 and 30 were active on the core switch. VLANs 10, 20 and 40 had to be created on the core switch too, after which DHCP worked.
- **Phone links stayed red:** the 2960 switches do not supply power to phones, so a power adapter module was added to each phone.

## Repository Contents

- Client requirements document
- IP addressing plan
- Physical and logical topology diagrams
- Month-end downtime constraint document
- Testing evidence screenshots (DHCP, DNS, trunking, cross-VLAN, VoIP)
- Packet Tracer `.pkt` file

## Project Status

- Milestone 1 (28 August 2026): complete
- Milestone 2 (2 October 2026): complete
- Final submission (16 October 2026): in progress (technical report and video demonstration)

## Reflection

*To be added after the video demonstration.*
