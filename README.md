# Enterprise Network Lab

A four-site simulated enterprise network built from scratch, covering routing and
switching, perimeter security, network access control, voice with measured QoS,
monitoring, and configuration automation — with the operational documentation
that would be needed to actually run it.

**Status:** Week 0 — setup
**Started:** September 4, 2026

---

## Summary

<!-- Fill this in at the end. Three or four sentences: what the network is,
     what it demonstrates, and the one or two results you are proudest of.
     Recruiters read this paragraph and nothing else. -->

## Headline results

<!-- Week 6: paste the QoS before/after table here. Numbers you measured
     yourself are the most persuasive thing in this repo. -->

| Metric          | No QoS | With QoS |
| --------------- | ------ | -------- |
| Jitter (ms)     |        |          |
| Packet loss (%) |        |          |
| MOS             |        |          |

---

## Architecture

<!-- Week 4+: embed the L3 diagram here -->

**Sites:** headquarters, two branch offices, one remote site over VPN
**Segmentation:** employee, servers, IoT, voice, guest

## Technology

| Layer               | Technology |
| ------------------- | ---------- |
| Simulation platform |            |
| Routing             |            |
| Switching           |            |
| Redundancy          |            |
| Firewall / VPN      |            |
| Access control      |            |
| Voice               |            |
| Monitoring          |            |
| Automation          |            |

---

## Repository layout

| Directory     | Contents                                             |
| ------------- | ---------------------------------------------------- |
| `topology/`   | Lab topology definitions (YAML / .pkt / .gns3)       |
| `configs/`    | Device configurations, commented                     |
| `docs/`       | IP plan, security policy, diagrams, lab setup guide  |
| `runbooks/`   | Tier-2 operational procedures                        |
| `incidents/`  | Incident writeups from failures caused and diagnosed |
| `monitoring/` | Monitoring stack config, dashboards, alert rules     |
| `automation/` | Ansible playbooks and scripts                        |
| `captures/`   | Curated Wireshark captures                           |
| `media/`      | Screenshots and demo recordings                      |

## Runbooks

<!-- Link each one as you write it -->

## Incidents

<!-- Link each one as you write it. Include the wrong turns. -->

---

## Reproducing this lab

See [docs/lab-setup.md](docs/lab-setup.md).
