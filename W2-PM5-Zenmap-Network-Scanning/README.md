# W2-PM5 — Local Network Host Discovery and Topology

## Overview

This module documents a basic host-discovery exercise performed with Zenmap (the graphical interface for Nmap) on Windows 11. The scan was limited to the practitioner's own personal mobile-hotspot network.

## Tools and Environment

| Item | Details |
|---|---|
| Operating system | Windows 11 |
| Scanner | Zenmap / Nmap |
| Nmap version | 7.98 |
| Npcap version | 1.83 |
| Scan type | Ping scan / host discovery |
| Target scope | Practitioner's own local hotspot subnet |

## Scan Method

The local IPv4 address, subnet mask, and default gateway were identified using `ipconfig`. The corresponding local subnet was then entered in Zenmap with the **Ping scan** profile.

Equivalent Nmap command:

```bash
nmap -sn <local-subnet>/24
```

The `-sn` option performs host discovery without a port scan. The scan was used to identify hosts that responded during the test.

## Observations

- Three hosts were reported as up during the scan.
- The responding devices were identified by correlating the scan output with the practitioner's knowledge of the connected laptop, second phone, and hotspot gateway.
- MAC address information was displayed for some discovered devices; it was not reported for every host.
- A Zenmap topology view was generated and saved as a PDF.

## Scope and Limitations

- The scan was restricted to the practitioner's own personal hotspot network.
- Host discovery indicates which devices responded to the probes at the time of scanning; it does not prove that no other devices were present.
- A ping scan does not enumerate open ports, identify running services, or establish that a host is vulnerable.
- MAC address visibility depends on the network path and discovery conditions.
- No exploitation, credential attacks, or intrusive vulnerability testing were performed.

## Evidence

Supporting screenshots are organized in the `screenshots/` directory:

- `host-details-mac.png` — discovered host details (MAC addresses redacted).
- `network-topology.png` — Zenmap network topology view.
- `nmap-scan-output.png` — host-discovery scan output.

The exported topology PDF is retained separately with the original assignment evidence.

## Disclaimer

This documentation is for educational purposes and independent cybersecurity learning. Network scanning should only be performed on networks owned by the practitioner or where explicit authorization has been granted.
