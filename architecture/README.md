# Lab Architecture

The lab uses six VirtualBox virtual machines on the isolated host-only network `192.168.56.0/24`.

| VM | OS / Role | Address |
|---|---|---|
| LAB-001 | CentOS Stream 9 | 192.168.56.10 |
| LAB-002 | Wazuh SIEM | 192.168.56.20 |
| LAB-003 | Windows 11 Pro | 192.168.56.30 |
| LAB-004 | Kali Linux | 192.168.56.40 |
| LAB-005 | Ubuntu Desktop | 192.168.56.50 |
| LAB-006 | Splunk SIEM | 192.168.56.60 |

**Supporting tools:** Wireshark on Windows host; Suricata for network traffic inspection; DFIR-IRIS case management; Python reporting. Their deployment and validation status should be recorded separately.

[View architecture infographic and details](https://lukedm0164-git.github.io/pages/lab-architecture.html)

## Validation checklist

- [ ] Verify IP and connectivity for all six VMs
- [ ] Document installed agents and Wazuh active status per endpoint
- [ ] Validate Splunk log ingestion
- [ ] Validate packet capture and network visibility
- [ ] Validate Suricata alerts
- [ ] Validate DFIR-IRIS case workflow
- [ ] Validate Python report generation

Mark each item complete only after testing.
