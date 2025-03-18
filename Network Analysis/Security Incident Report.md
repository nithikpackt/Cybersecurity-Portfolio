## Scenario:

You are a cybersecurity analyst for yummyrecipesforme.com, a website that sells recipes and cookbooks. A former employee has decided to lure users to a fake website with malware. 

The former employee/ hacker executed a brute force attack to gain access to the web host. They repeatedly entered several known default passwords for the administrative account until they correctly guessed the right one. After they obtained the login credentials, they were able to access the admin panel and change the website’s source code. They embedded a javascript function in the source code that prompted visitors to download and run a file upon visiting the website. After embedding the malware, the hacker changed the password to the administrative account. When customers download the file, they are redirected to a fake version of the website that contains the malware. 

Several hours after the attack, multiple customers emailed yummyrecipesforme’s helpdesk. They complained that the company’s website had prompted them to download a file to access free recipes. The customers claimed that, after running the file, the address of the website changed and their personal computers began running more slowly. 

In response to this incident, the website owner tries to log in to the admin panel but is unable to, so they reach out to the website hosting provider. You and other cybersecurity analysts are tasked with investigating this security event.

To address the incident, you create a sandbox environment to observe the suspicious website behavior. You run the network protocol analyzer tcpdump, then type in the URL for the website, yummyrecipesforme.com. As soon as the website loads, you are prompted to download an executable file to update your browser. You accept the download and allow the file to run. You then observe that your browser redirects you to a different URL, greatrecipesforme.com, which contains the malware.  

The logs show the following process:

1. The browser initiates a DNS request: It requests the IP address of the yummyrecipesforme.com URL from the DNS server.

2. The DNS replies with the correct IP address. 

3. The browser initiates an HTTP request: It requests the yummyrecipesforme.com webpage using the IP address sent by the DNS server.

4. The browser initiates the download of the malware.

5. The browser initiates a DNS request for greatrecipesforme.com.

6. The DNS server responds with the IP address for greatrecipesforme.com.

7. The browser initiates an HTTP request to the IP address for greatrecipesforme.com.

A senior analyst confirms that the website was compromised. The analyst checks the source code for the website. They notice that javascript code had been added to prompt website visitors to download an executable file. Analysis of the downloaded file found a script that redirects the visitors’ browsers from yummyrecipesforme.com to greatrecipesforme.com. 

The cybersecurity team reports that the web server was impacted by a brute force attack. The disgruntled hacker was able to guess the password easily because the admin password was still set to the default password. Additionally, there were no controls in place to prevent a brute force attack. 

Your job is to document the incident in detail, including identifying the network protocols used to establish the connection between the user and the website.  You should also recommend a security action to take to prevent brute force attacks in the future.

You can access the tcpdump traffic log here:

[tcpdump traffic log](https://d3c33hcgiwev3.cloudfront.net/DfNS2bS8SFSX2LAq8wdGew_2e223b94ae5c4f7dbf841cee85b247f1_tcpdump-traffic-log.docx?Expires=1742428800&Signature=UEd0sKo-kZFWcDilFsV3uApSd2WGapQMbmJ8KtohICoz85gClbsVlkg6vUpxbclG3F2ZW7UwTQ5nzaNuIvjxRdnmjxtqQq-5berMCvCqr-hjW0JfG1AHQnCjB-njIWpeXD6bPSGfHvKmk8R-y-QMtzHMEEAN90DGJxPrbFS1Xb4_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)

## Security Incident Report:

| Section 1: Identify the network protocol involved in the incident |
|---|
| The network protocols involved in this incident are: |
| DNS (Domain Name System): Used to translate the domain names (yummyrecipesforme.com, greatrecipesforme.com) to their corresponding IP addresses. |
| HTTP (Hypertext Transfer Protocol): Used for communication between the browser and the web servers to request and receive web pages and other content. |

| Section 2: Document the incident |
|---|
| **Incident Summary:** |
| Yummyrecipesforme.com experienced a security breach resulting in website defacement and malware distribution. A former employee gained unauthorized access to the web server's administrative panel via a brute-force attack on the admin account, exploiting the use of a default password. |
| **Timeline of Events:** |
| 1. Unauthorized Access: The attacker successfully brute-forced the administrative account password, gaining access to the web server's admin panel. |
| 2. Code Modification: The attacker modified the website's source code, embedding a JavaScript function designed to prompt website visitors to download and execute a file. |
| 3. Credential Change: The attacker changed the administrative account password to prevent the website owner from accessing the admin panel. |
| 4. Malware Distribution: Website visitors who downloaded and ran the file were redirected to a fake website (greatrecipesforme.com) containing malware. |
| 5. User Reports: Multiple customers contacted yummyrecipesforme's helpdesk, reporting suspicious download prompts and subsequent redirection to a different website with performance issues on their computers. |
| 6. Detection and Investigation: The website owner, unable to access the admin panel, contacted the website hosting provider. Cybersecurity analysts were tasked with investigating the incident. |
| 7. Sandbox Analysis: Analysts created a sandbox environment to observe the website's behavior. Using tcpdump, they confirmed the malicious redirection. |
| 8. Log Analysis: Logs revealed the following process: |
| - DNS requests for yummyrecipesforme.com and greatrecipesforme.com. |
| - HTTP requests to yummyrecipesforme.com and greatrecipesforme.com. |
| 9. Malware download initiation. |
| 10. Source Code Review: A senior analyst confirmed the presence of malicious JavaScript code in the website's source code, which triggered the download and redirection. |
| 11. Root Cause Analysis: The cybersecurity team determined that the root cause was a brute-force attack due to the use of a default password and the absence of brute-force prevention controls. |
| **Impact:** |
| Website defacement<br> Malware distribution<br> Compromised user systems<br> Reputational damage to yummyrecipesforme.com<br> Loss of customer trust<br> |

