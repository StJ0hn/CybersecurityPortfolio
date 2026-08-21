# TCP SYN Flood Incident Analysis

A hands-on network security case study completed as part of the Google Cybersecurity Professional Certificate.

## Scenario

A company web server became unavailable after receiving an abnormally high number of TCP SYN requests from an unknown IP address. Using network logs captured with Wireshark, I analyzed the traffic to identify the attack, explain its impact, and document the findings in an incident report.

## Objective

- Identify the network attack.
- Analyze packet behavior.
- Explain how the attack affected the web server.
- Document findings using an incident response format.

## Investigation Process

1. Reviewed the incident scenario.
2. Analyzed TCP/HTTP logs exported from Wireshark.
3. Identified an abnormal volume of TCP SYN packets.
4. Correlated the evidence with TCP connection behavior.
5. Concluded the incident was a TCP SYN Flood (DoS) attack.

## Key Findings

- Large number of TCP SYN packets from an unknown IP.
- Server resources became exhausted while processing pending connections.
- Legitimate users experienced connection timeout errors.
- Temporary containment included isolating the server and blocking the source IP.

## Technical Concepts Demonstrated

- TCP Three-Way Handshake
- SYN Flood Attack
- Denial of Service (DoS)
- Packet Analysis
- Log Interpretation
- Incident Documentation

## Skills Demonstrated

- Network traffic analysis
- Security incident identification
- Evidence-based reasoning
- Technical reporting
- Wireshark log interpretation