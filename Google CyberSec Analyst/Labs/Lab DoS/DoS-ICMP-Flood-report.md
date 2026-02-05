# Incident Report – ICMP Flood DoS
**Instructions**
Throughout this course, you will be able to use this template to record your findings after completing an activity or to take notes on what you have learned about a specific tool or concept.You can also use this chart as a way to practice applying the NIST framework to different situations you encounter.

## Summary

The organization suffered a Denial-of-Service (DoS) attack based on an ICMP packet flood, which resulted in the total unavailability of internal network services for a period of two hours. During the incident, internal systems were unable to access essential network resources, directly impacting business continuity.
The incident management team contained the event by blocking incoming ICMP traffic and temporarily disabling non-critical services. Analysis of the log records indicated that the attack was enabled by an improper firewall configuration, allowing a malicious actor to exploit this vulnerability to execute the attack against the company's network.


## Identify
**Type of attack:** DoS (Denial of Service)
**Attack vector:** ICMP Flood (Ping Flood)
**Systems affected:**Internal network infrastructure, internal services, and access to external resources.

## Protect
Implement network access control policies through IP address validation and anti-spoofing mechanisms to prevent the acceptance of ICMP packets with spoofed source addresses.
Configure the firewall to filter ICMP traffic, applying specific rules that allow only the types of messages strictly necessary for the network to function.
Implement rate limits (rate limiting) and traffic volume controls for ICMP packets, reducing the impact of flood attempts and preventing network resource saturation.
Establish and maintain a secure firewall configuration baseline, ensuring that critical rules, policies, and parameters are properly standardized, documented, and reviewed periodically.
Segmenting the network into logical security zones, separating critical systems, internal services, and external access areas, in order to contain the spread of attacks and reduce the damage caused by a potential denial-of-service incident.


## Detect
Implement the use of SIEM tools integrated with IDS systems to continuously monitor network traffic, identifying anomalous ICMP packet patterns, such as volume spikes and excessive requests. Correlate events and logs from network devices to generate automatic alerts and notify the security team about potential DoS attacks at an early stage.

## Respondent
The security team contained the incident by immediately blocking incoming ICMP traffic at the firewall, interrupting the attack vector. As a mitigation measure, non-critical network services were temporarily disabled, reducing infrastructure overload and prioritizing environmental stability.
During the incident, log records and firewall configuration were analyzed to identify the source of the attack and the exploited configuration flaw, as well as to keep the responsible areas informed about the event status and the actions taken.


## Recover
After containing the attack, the security team restored critical network services in a controlled manner, ensuring the resumption of essential operations. Subsequently, the new firewall rules implemented during the incident were reviewed and validated to confirm the effectiveness of the measures taken. The stability and integrity of the environment were verified through connectivity tests and network traffic monitoring. Finally, the incident was formally closed, with updated security rules and procedures incorporating the corrections made into the organization's security processes.

## Reflections / Notes
 **Event analyzed according to CSF-NIST.**

 ## Proteger
