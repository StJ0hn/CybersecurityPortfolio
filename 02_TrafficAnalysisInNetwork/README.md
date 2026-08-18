# DNS and ICMP Traffic Analysis

## Description

Network traffic analysis activity from the **Google Cybersecurity Certificate**, covering packet inspection with `tcpdump`, DNS troubleshooting, ICMP error interpretation, and cybersecurity incident reporting.

## Overview

This activity simulates the investigation of a network incident where users were unable to access the fictional website **www.yummyrecipesforme.com**. Using a `tcpdump` packet capture, the objective is to identify the network protocols involved, interpret packet metadata and error messages, determine the affected service, and document the findings in a structured incident report.

The analysis focuses on how DNS queries over UDP resulted in ICMP **Destination Port Unreachable** messages, indicating a failure affecting the DNS service on UDP port 53.

## Topics

- Network traffic analysis with `tcpdump`
- DNS resolution workflow
- UDP packet inspection
- ICMP Destination Unreachable messages
- Incident analysis and reporting

## Learning Objectives

- Analyze packet captures using `tcpdump`
- Identify the roles of IP, UDP, DNS, and ICMP during network communication
- Interpret timestamps, source and destination addresses, ports, and protocol flags
- Determine the affected network service based on packet evidence
- Produce a structured cybersecurity incident report

## Repository Structure

```text
02_TrafficAnalysisInNetwork/
├── README.md
└── CybersecurityIncidentReport.pdf
```

## Investigation Summary

The packet capture revealed that the browser successfully transmitted DNS queries over **UDP**, but the DNS server repeatedly responded with **ICMP Destination Port Unreachable** messages. The recurring **"UDP port 53 unreachable"** error indicates that the DNS service was unavailable, preventing domain name resolution and consequently blocking access to the website.

## References

- Google Cybersecurity Certificate (Coursera) — Network Traffic Analysis module
- `tcpdump` documentation
- Internet Control Message Protocol (ICMP)
- Domain Name System (DNS)

## License

This activity is part of the [Cybersecurity Portfolio](../) repository and is licensed under the MIT License — see the root [LICENSE](../LICENSE) for details.