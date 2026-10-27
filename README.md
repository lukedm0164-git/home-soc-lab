# Home SOC Lab — Luke Morris

**A documented, six-VM cybersecurity lab for defensive security operations, threat detection, incident investigation, and automation.**

[Portfolio website](https://lukedm0164-git.github.io/) · [Lab architecture](https://lukedm0164-git.github.io/pages/lab-architecture.html) · [GitHub profile](https://github.com/lukedm0164-git)

## Project status

**In progress.** The architecture describes the intended integrated environment. Individual systems and workflows are documented as they are configured and validated; a listed tool does not imply that its integration is complete.

## Lab architecture

| ID | System | Host-only IP | Purpose |
|---|---|---|---|
| LAB-001 | CentOS Stream 9 | `192.168.56.10` | Monitored Linux server |
| LAB-002 | Wazuh SIEM | `192.168.56.20` | Endpoint log collection, detection and analysis |
| LAB-003 | Windows 11 Pro | `192.168.56.30` | Monitored Windows workstation |
| LAB-004 | Kali Linux | `192.168.56.40` | Controlled attack simulation |
| LAB-005 | Ubuntu Desktop | `192.168.56.50` | Monitored Linux workstation |
| LAB-006 | Splunk SIEM | `192.168.56.60` | Log search and analysis |

**VirtualBox host-only network:** `192.168.56.0/24`

Additional tools in the architecture: Suricata IDS (network traffic monitoring), Wireshark (packet capture/analysis on Windows host), DFIR-IRIS (case management), and Python (report automation). These tools do not represent additional numbered VMs.

## Repository guide

| Folder | Contents |
|---|---|
| [architecture/](architecture/README.md) | Network design, IP inventory, configuration notes |
| [setup-guides/](setup-guides/README.md) | Reproducible configuration and validation procedures |
| [incident-reports/](incident-reports/README.md) | Evidence-led incident investigations |
| [detection-rules/](detection-rules/README.md) | Wazuh, Splunk and network detection logic |
| [scripts/](scripts/README.md) | Python and PowerShell automation |
| [screenshots/](screenshots/README.md) | Sanitized visual evidence for reports |
| [sample-logs/](sample-logs/README.md) | Synthetic or sanitized data for reproducible exercises |
| [templates/](templates/incident-report-template.md) | Reusable documentation templates |

## Documentation standard

Every completed investigation should explain the question, lab conditions, commands or queries, evidence and timestamps, findings, limitations, and what was learned. Planned work stays labeled **planned** until validated.

This repository contains no real-world targets, credentials, secrets, or unredacted personal data.
