# Website compromise incident analysis

A cybersecurity portfolio project based on the practice assignment **Apply OS hardening techniques**. This is a simulated training scenario, not a real incident or a live investigation I performed.

## Project overview

I reviewed a supplied scenario and tcpdump traffic log for yummyrecipesforme.com, identified HTTP traffic, documented the incident, and considered controls to reduce the risk of unauthorised admin access.

In the scenario, an attacker guessed a default admin password, changed the website source code to prompt a malicious download, and changed the admin password. After running the downloaded file, visitors were redirected to greatrecipesforme.com.

## My report

[Read the completed security incident report](security-incident-report.pdf).

The report covers the network protocol, the incident and its investigation, and recommendations concerning password security and two-factor authentication. The supplied final PDF is preserved unchanged.

## What the traffic shows

- DNS resolves yummyrecipesforme.com to 203.0.113.22.
- TCP establishes a connection, followed by an HTTP GET request.
- A later DNS lookup resolves greatrecipesforme.com to 192.0.2.172.
- Another TCP connection and HTTP GET request follow for the second domain.

The log supports communication with both websites. The supplied scenario provides the findings about password guessing, source-code changes, downloaded-file behaviour, and malware. The excerpt alone does not prove those findings or the cause of the redirect.

## What I learned

- How DNS, TCP and HTTP work together when a browser accesses a website.
- How to recognise a TCP three-way handshake and an HTTP GET request in tcpdump output.
- How to distinguish observed network evidence from information provided by an incident scenario.
- How to explain why an additional authentication factor helps when a password is guessed.

## Materials and scope

The course-provided scenario, instructions, exemplar and original traffic-log PDF are reference materials and are not redistributed here. The report describes actions performed by the fictional analysts in the exercise. No malware was downloaded or executed for this portfolio project.
