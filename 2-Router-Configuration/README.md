# Day 2 - Router Configuration

## Objective
Configure a Cisco router to connect
two separate LANs.

## Network Topology
Topology screenshot will be added.

## IP Addressing

| Device | IP Address |
|---|---|
| R1 G0/0 | 10.10.10.1/24 |
| R1 G0/1 | 10.10.20.1/24 |
| PC1 | 10.10.10.10/24 |
| PC2 | 10.10.20.10/24 |

## Router Configuration
To be documented.

## Connectivity Testing
To be verified.

## Troubleshooting
To be documented.

## Lessons Learned
To be completed.


## Router Interface Configuration

| Interface | IP Address | Status |
|---|---|---|
| G0/0 | 10.10.10.1/24 | Up/Up |
| G0/1 | 10.10.20.1/24 | Up/Up |

## Routing Table

| Route | Network | Interface |
|---|---|---|
| C | 10.10.10.0/24 | G0/0 |
| L | 10.10.10.1/32 | G0/0 |
| C | 10.10.20.0/24 | G0/1 |
| L | 10.10.20.1/32 | G0/1 |

## Verification Commands

- show ip interface brief
- show ip route
- show running-config
