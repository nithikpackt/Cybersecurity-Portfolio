## Scenario

You work as a security analyst for a travel agency that advertises sales and promotions on the company’s website. The employees of the company regularly access the company’s sales webpage to search for vacation packages their customers might like. 

One afternoon, you receive an automated alert from your monitoring system indicating a problem with the web server. You attempt to visit the company’s website, but you receive a connection timeout error message in your browser.

You use a packet sniffer to capture data packets in transit to and from the web server. You notice a large number of TCP SYN requests coming from an unfamiliar IP address. The web server appears to be overwhelmed by the volume of incoming traffic and is losing its ability to respond to the abnormally large number of SYN requests. You suspect the server is under attack by a malicious actor. 

You take the server offline temporarily so that the machine can recover and return to a normal operating status. You also configure the company’s firewall to block the IP address that was sending the abnormal number of SYN requests. You know that your IP blocking solution won’t last long, as an attacker can spoof other IP addresses to get around this block. You need to alert your manager about this problem quickly and discuss the next steps to stop this attacker and prevent this problem from happening again. You will need to be prepared to tell your boss about the type of attack you discovered and how it was affecting the web server and employees.

[![Wireshark Capture](https://iconduck.com/icons/110378/wireshark?shared)](https://docs.google.com/spreadsheets/d/1enpRzrIao3J2Lp2tOI0hmu1Cu7D7CjLGhFAiTiR9J64/edit?gid=218501934#gid=218501934)

| Section 1: Identify the type of attack that may have caused this network interruption |
|---|
| - One potential explanation for the website's connection timeout error message is: **DOS attack using SYN flood** |
| - The logs show that: a large number of **SYN requests** flooding the server |
| - This event could be: **TCP-SYN flood attack** |

| Section 2: Explain how the attack is causing the website to malfunction |
|---|
| - When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake: |
| 1. SYN: The client initiates the connection by sending a SYN packet to the server |
| 2. SYN-ACK: Upon receiving the SYN packet, the server responds with a SYN-ACK packet. |
| 3. ACK: The client receives the SYN-ACK packet and sends an ACK packet back to the server. |
| |
| 203.0.113.0 is the source IP of the attacker. For now, we can take down the server and setup firewall rules to block the IP in question. But I reckon, that would only be a temporary solution |
| - Explain what happens when a malicious actor sends a large number of SYN packets all at once: |
| When a malicious actor floods the server with a large number of SYN packets, it overloads the server and it stops working. |
| - Explain what the logs indicate and how that affects the server: |
| When looking at Wireshark logs. From line 80, the attacker's SYN flood makes it impossible for the server to operate and serve the webpage, causing an outage. |





