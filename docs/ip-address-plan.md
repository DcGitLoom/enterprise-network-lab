# IP Address Plan

> Complete this in **Week 2**. Every later week depends on it. Design it once,
> with growth room, rather than inventing subnets as you go.

**Supernet:** 10.0.0.0/8
**Allocation scheme:** 10.<site>.<vlan>.0/24

## Sites

| ID | Site | Role | Supernet |
|---|---|---|---|
| 1 | Headquarters | Core + datacenter | 10.1.0.0/16 |
| 2 | Branch A | Office | 10.2.0.0/16 |
| 3 | Branch B | Office | 10.3.0.0/16 |
| 4 | Remote | VPN site | 10.4.0.0/16 |

## VLANs (consistent across all sites)

| VLAN | Name | Purpose | Third octet |
|---|---|---|---|
| 10 | employee | User workstations | 10 |
| 20 | servers | Internal services | 20 |
| 30 | iot | Cameras, sensors, printers | 30 |
| 40 | voice | IP phones | 40 |
| 50 | guest | Untrusted | 50 |
| 99 | quarantine | Failed 802.1X | 99 |

## Per-site allocations

| Site | VLAN | Subnet | Gateway | DHCP range |
|---|---|---|---|---|
| HQ | 10 | 10.1.10.0/24 | 10.1.10.1 | .100–.200 |
| | | | | |

## Point-to-point links

| Link | Subnet | A side | B side |
|---|---|---|---|
| HQ ↔ Branch A | 10.255.1.0/30 | .1 | .2 |
| | | | |

## Loopbacks

| Device | Loopback |
|---|---|
| | |

## Reserved / do not use

| Range | Reason |
|---|---|
| | |
