# W2-PM1 — Domain Footprinting

## Overview

This module documents practical exercises in domain footprinting using command-line tools available in Kali Linux. The activities focused on gathering and examining publicly available information about the target domain, `networkwalks.com`.

## Tools Used

| Tool | Purpose |
|---|---|
| WHOIS | Retrieve domain registration and registrar information |
| WhatWeb | Identify web technologies and server-related information |
| Nslookup | Query DNS records and resolve domain names |
| cURL | Inspect HTTP response headers |
| WAFW00F | Identify the presence of a Web Application Firewall (WAF) |
| DNSRecon | Enumerate DNS records and related configuration information |

## Practical Activities

The following activities were completed:

1. **WHOIS:** Examined domain registration details, registrar information, domain status, name servers, and DNSSEC status.
2. **WhatWeb:** Fingerprinted the target website to identify technologies and web server information.
3. **Nslookup:** Queried A, NS, and MX records to examine domain name resolution.
4. **cURL:** Inspected HTTP response headers using HEAD requests.
5. **WAFW00F:** Checked whether a Web Application Firewall could be identified.
6. **DNSRecon:** Performed DNS enumeration to collect available DNS records and related information.

## Scope and Limitations

- The exercises focused on publicly available domain, DNS, and HTTP response information.
- The target was examined for footprinting and information-gathering purposes.
- Tool output represents observations at the time of testing and may change.
- Technology identification does not establish that a component is vulnerable.
- The presence of a WAF does not establish the effectiveness of its protection.
- No exploitation, credential attacks, or intrusive vulnerability testing were performed.

## Evidence and Documentation

Each tool has its own directory containing practical notes and supporting screenshots.

- `whois/`
- `whatweb/`
- `nslookup/`
- `curl/`
- `wafw00f/`
- `dnsrecon/`

The WHOIS directory contains multiple screenshots because of the length of its output.

## Disclaimer

This documentation is intended for educational purposes and independent cybersecurity learning. Footprinting activities should only be conducted against domains and systems where testing is permitted or explicitly authorized.
