Scenario
--------

Review the scenario below. Then complete the step-by-step instructions.

You are a cybersecurity analyst working for a multimedia company that offers web design services, graphic design, and social media marketing solutions to small businesses. Your organization recently experienced a DDoS attack, which compromised the internal network for two hours until it was resolved.

During the attack, your organization’s network services suddenly stopped responding due to an incoming flood of ICMP packets. Normal internal network traffic could not access any network resources. The incident management team responded by blocking incoming ICMP packets, stopping all non-critical network services offline, and restoring critical network services. 

The company’s cybersecurity team then investigated the security event. They found that a malicious actor had sent a flood of ICMP pings into the company’s network through an unconfigured firewall. This vulnerability allowed the malicious attacker to overwhelm the company’s network through a distributed denial of service (DDoS) attack. 

To address this security event, the network security team implemented: 

*   A new firewall rule to limit the rate of incoming ICMP packets
    
*   Source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets
    
*   Network monitoring software to detect abnormal traffic patterns
    
*   An IDS/IPS system to filter out some ICMP traffic based on suspicious characteristics
    

As a cybersecurity analyst, you are tasked with using this security event to create a plan to improve your company’s network security, following the National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF). You will use the CSF to help you navigate through the different steps of analyzing this cybersecurity event and integrate your analysis into a general security strategy. We have broken the analysis into different parts in the template below. You can explore them here:

*   **Identify** security risks through regular audits of internal networks, systems, devices, and access privileges to identify potential gaps in security. 
    
*   **Protect** internal assets through the implementation of policies, procedures, training and tools that help mitigate cybersecurity threats. 
    
*   **Detect** potential security incidents and improve monitoring capabilities to increase the speed and efficiency of detections. 
    
*   **Respond** to contain, neutralize, and analyze security incidents; implement improvements to the security process. 
    

**Recover** affected systems to normal operation and restore systems data and/or assets that have been affected by an incident.


| **Summary**      |   | 
|------------------|---|
| **Identify**     | Threat actor targeted the company with an ICMP flood attack resulting in complete network unavaialability and caused diruption in major staff operations. Internal network needs to be fixed brought back online  |  
| **Protect**      |  Maintaining a robust security posture requires the cybersecurity team to be immediately alerted to any attacks. As all staff utilize the internal network, a critical step is to establish a new firewall rule that restricts the rate of incoming ICMP packets. This rule must be consistently updated to address evolving attack trends. The cybersecurity team should also diligently monitor and update all devices, operating systems, and software to ensure the deployment of the latest security updates. Moreover, the implementation of an IDS/IPS system will enable the filtering of ICMP traffic exhibiting suspicious characteristics, further strengthening defenses |   
| **Detect**       | The cybersecurity team can enhance defenses by configuring source IP address verification on the firewall. They should also analyze spoofed IP addresses on incoming ICMP packets using tools like Wireshark or TCPdump. Furthermore, implementing network monitoring software (SIEM, such as Splunk or LogRhythm) is crucial for detecting abnormal traffic patterns. Implementing an IDS will also be a good option here  |   
| **Respond**      |  The cybersecurity team needs to establish robust risk management protocols for future security incidents. This framework will serve as a standard operating guide when threats emerge. In the event of an incident, the team will immediately inform end-users of necessary next steps and take swift action to contain the spread of malicious files by isolating affected systems. They will then focus on restoring any disrupted critical systems and services. Post-incident, a thorough analysis of network logs will be conducted to identify suspicious and abnormal activity. Finally, all incidents must be reported to upper management and legal authorities in compliance with relevant laws and regulations. | 
| **Recover**      | Addressing ICMP flooding is paramount for maintaining uninterrupted network services. The team should leverage a firewall to block these attacks. In practice, critical network services take precedence, allowing non-critical networks to temporarily go offline if necessary. Once the ICMP packet flood has passed, all non-critical network systems and services can be restored.  |  
