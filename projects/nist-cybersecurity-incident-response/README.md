# NIST Cybersecurity Framework: Incident Response Analysis

An educational incident analysis from the Google Cybersecurity Certificate. This project applies the NIST Cybersecurity Framework (CSF) functions to a simulated ICMP flood denial-of-service (DoS) scenario.

## Report

[Read the incident report (PDF)](Incident%20report%20analysis.pdf)

## Scenario

The coursework scenario describes an ICMP packet flood that disrupted access to a fictional multimedia company's internal network services for two hours. The report identifies an unconfigured firewall as a contributing weakness and discusses steps to contain the disruption and restore critical services.

## NIST CSF analysis

- **Identify:** Recognise the ICMP flood, affected network services, and firewall configuration gap described in the scenario.
- **Protect:** Recommend limiting ICMP request rates and validating source addresses; the report also discusses network monitoring and an intrusion prevention system.
- **Detect:** Use firewall controls, network monitoring, and intrusion detection to identify abnormal ICMP traffic and possible spoofed addresses.
- **Respond:** The scenario describes blocking incoming ICMP traffic, taking non-critical services offline, restoring critical services, and reviewing suspicious activity.
- **Recover:** Return services to normal after the attack stops, apply the proposed traffic controls, and monitor for renewed suspicious traffic.

## Skills demonstrated

- Applying the NIST CSF functions to an incident scenario
- Describing an ICMP flood and its service availability impact
- Connecting firewall controls and monitoring to incident response
- Communicating response and recovery recommendations

## Scope

This is a simulated coursework exercise, not a real incident or assessment of a live organisation. The controls and response actions are described in the assignment scenario and report; this portfolio entry does not claim that I configured, deployed, or tested them in a live environment.
