# SYN Flood Analysis: Website Service Interruption

A separate Google Cybersecurity Certificate coursework project analysing a suspected TCP SYN flood against a fictional travel agency website. I reviewed supplied packet-log evidence and documented the likely attack and its impact on legitimate users.

## Report

[Read the cybersecurity incident report (PDF)](syn-flood-incident-report.pdf)

## Scenario

The scenario describes a monitoring alert, website connection timeouts, and an unusually large number of SYN requests from an unfamiliar IP address. Employees could not reliably access the sales webpage to find vacation packages for customers.

## Findings

- Repeated SYN requests from the apparent source 203.0.113.0 target 192.0.2.1 on TCP port 443.
- Packets 57, 59 and 61 contain SYN requests. Packet 64 is a SYN/ACK reply, followed by another SYN in packet 66 without a final ACK visible in between.
- Connection resets and an HTTP 504 Gateway Time-out response indicate service problems affecting other clients.
- The pattern is consistent with a suspected SYN flood denial-of-service (DoS) attack. The supplied log alone does not confirm resource exhaustion or establish a distributed attack.

## How the attack affects availability

A normal TCP connection starts with SYN, SYN/ACK and ACK. In a SYN flood, repeated requests leave handshakes unfinished. Tracking pending connections can consume server resources and prevent legitimate visitors from connecting.

## Skills demonstrated

- Interpreting supplied packet logs and TCP flags
- Following the TCP three-way handshake across interleaved conversations
- Connecting suspicious traffic patterns with service disruption
- Explaining denial-of-service behaviour and documenting evidence with appropriate uncertainty

## Scope

This is analysis of a simulated coursework scenario, not a live incident or an attack I conducted. The scenario describes temporarily taking the server offline and blocking the source IP; I did not perform these actions. The report focuses on identifying the suspected attack and explaining its impact.
