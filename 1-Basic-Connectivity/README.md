# 1 - Basic Network Connectivity

## Objective
Configure a basic network using PCs,
a switch, and a router.

## Tasks
- Configure IP addresses
- Configure default gateways
- Enable router interfaces
- Test connectivity using ping

## Troubleshooting
Corrected an incorrect default gateway
and verified successful connectivity.

## Network Topology

![1 Network Topology](network-topology.png)

## IP Addressing

| Device | IP Address | Subnet Mask | Default Gateway |
|---|---|---|---|
| PC1 | 192.168.10.10 | 255.255.255.0 | 192.168.10.1 |
| PC2 | 192.168.20.10 | 255.255.255.0 | 192.168.20.1 |

## Network Verification

Connectivity between PC1 and PC2
will be tested using ICMP ping.

## Router R1 Configuration

| Interface | IP Address | Status |
|---|---|---|
| G0/0 | 192.168.10.1/24 | Up/Up |
| G0/1 | 192.168.20.1/24 | Up/Up |
| G0/2 | Unassigned | Admin Down |

### Routing
R1 connects two LANs:
- 192.168.10.0/24
- 192.168.20.0/24

Both configured interfaces are operational.

## Switch Configuration

### Interface Status

| Interface | Status | VLAN |
|---|---|---|
| Fa0/1 | Connected | 1 |
| Gig0/1 | Connected | 1 |
| Other ports | Not connected | 1 |

### VLAN Configuration
- VLAN 1 is active.
- All ports belong to VLAN 1.
- No additional VLANs configured.

### Verification Commands
show interfaces status
show vlan brief
