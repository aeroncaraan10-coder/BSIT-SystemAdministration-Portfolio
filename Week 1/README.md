# Week 2: Enterprise Infrastructure Planning for a Startup Company

## Student Information

- **Name:** Caraan, Aeron Abriel V.
- **Course:** BSIT – ITEP 414: System Administration and Maintenance
- **Section:** To be added
- **Date:** Week 2

## Network Topology

![ABC Startup Solutions network topology](images/ABC-Startup-Solutions-Network-Topology.svg)

## ABC Startup Solutions: Infrastructure Plan

### 1. Company Overview

ABC Startup Solutions is a growing company with departments for Administration, Finance, Sales, and IT. Its infrastructure should provide secure internet access, shared company resources, reliable backups, and room to expand as the team grows.

### 2. Network Segmentation and IP Plan

| Network | VLAN | Example subnet | Purpose |
|---|---:|---|---|
| Administration | 10 | `192.168.10.0/24` | Administration workstations |
| Finance | 20 | `192.168.20.0/24` | Finance workstations |
| Sales | 30 | `192.168.30.0/24` | Sales workstations |
| IT and Management | 40 | `192.168.40.0/24` | IT workstations and network management |
| Servers | 50 | `192.168.50.0/24` | Shared services and internal servers |
| Staff Wi-Fi | 60 | `192.168.60.0/24` | Employee wireless devices |
| Guest Wi-Fi | 70 | `192.168.70.0/24` | Visitor internet access only |

The firewall should control traffic between VLANs. Guest Wi-Fi should not be able to access company devices or servers.

### 3. Proposed Infrastructure

- **Firewall/router:** Filters internet traffic, supports VPN access, and applies network rules.
- **Managed switch:** Connects office devices and separates departments using VLANs.
- **Wireless access points:** Provide staff and guest Wi-Fi on separate networks.
- **File and print services:** Provide authorized staff access to shared documents and printers.
- **Backup storage:** Keeps scheduled copies of important company data.
- **Monitoring and logging:** Helps IT staff review device status and investigate issues.
- **Cloud services:** Email and collaboration tools can be hosted through a business cloud provider.

### 4. Security and Maintenance

- Give each employee an individual account and only the access needed for their role.
- Require strong passwords and multifactor authentication for cloud and remote access.
- Keep operating systems, applications, firewall firmware, and network equipment updated.
- Use endpoint protection on company computers.
- Back up important data regularly and periodically check that files can be restored.
- Review firewall rules, user accounts, and logs as part of routine maintenance.
- Document device names, IP assignments, administrator access, and recovery procedures.

### 5. Growth Plan

The design can expand by adding switch ports, wireless access points, user devices, or cloud services. New departments can receive their own VLAN and subnet. Before expansion, IT should review firewall capacity, backup storage, available IP addresses, and internet bandwidth.

### 6. Summary

This plan separates department traffic, protects internal resources through firewall rules, and includes shared services, backups, and monitoring. It provides ABC Startup Solutions with a manageable network that can grow with the company.
