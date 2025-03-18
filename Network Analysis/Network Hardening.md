## Scenario:

Review the following scenario. Then complete the step-by-step instructions.

You are a security analyst working for a social media organization. The organization recently experienced a major data breach, which compromised the safety of their customers’ personal information, such as names and addresses. Your organization wants to implement strong network hardening practices that can be performed consistently to prevent attacks and breaches in the future. 

After inspecting the organization’s network, you discover four major vulnerabilities. The four vulnerabilities are as follows:

1. The organization’s employees' share passwords.

2. The admin password for the database is set to the default.

3. The firewalls do not have rules in place to filter traffic coming in and out of the network.

4. Multifactor authentication (MFA) is not used. 

If no action is taken to address these vulnerabilities, the organization is at risk of experiencing another data breach or other attacks in the future. 

In this activity, you will write a security risk assessment to analyze the incident and explain what methods can be used to further secure the network.

| Part 1: Select up to three hardening tools and methods to implement |
|---|
| Here are three crucial hardening methods to implement: |
| 1. Strong Password Policies and Management: This addresses the issues of shared passwords and default passwords. |
| 2. Firewall Configuration and Rule Implementation: This directly addresses the lack of firewall rules. |
| 3. Multi-Factor Authentication (MFA) Enforcement: This addresses the absence of MFA. |

# Part 2: Explain your recommendations

Here's an explanation of why these recommendations are critical and how they enhance the organization's security posture:

**Strong Password Policies and Management:**

* **The Problem:**
    * Employees sharing passwords creates a significant vulnerability. If one account is compromised, multiple systems and data become at risk.
    * Default passwords are a well-known security risk, making brute-force attacks trivially easy.
* **The Solution:**
    * Implement a strong password policy that includes:
        * Complexity Requirements: Passwords must meet minimum length, and include a mix of uppercase letters, lowercase letters, numbers, and special characters.
        * Regular Password Changes: Enforce regular password changes (e.g., every 90 days).
        * Prohibition of Password Sharing: Explicitly prohibit password sharing in company policy and enforce it through technical controls where possible.
        * Password Managers: Encourage or even mandate the use of password managers to help employees create and store strong, unique passwords for each account.
    * Change all default passwords immediately, especially for administrative accounts and databases.
* **Security Benefit:**
    * Reduces the risk of unauthorized access due to weak, shared, or default passwords.
    * Limits the impact of a single compromised account.

**Firewall Configuration and Rule Implementation:**

* **The Problem:**
    * Firewalls without properly configured rules are ineffective. They essentially act as open doors, allowing potentially malicious traffic to enter and sensitive data to leave the network freely.
* **The Solution:**
    * Implement a well-defined firewall policy and configure firewall rules based on the principle of least privilege. This includes:
        * Ingress Filtering: Rules to carefully control incoming traffic, blocking unsolicited connections and only allowing necessary traffic through specific ports and protocols.
        * Egress Filtering: Rules to monitor and control outgoing traffic, preventing data exfiltration and unauthorized communication.
        * Regular Review and Updates: Regularly review and update firewall rules to ensure they remain effective and aligned with the organization's security needs.
        * Intrusion Detection/Prevention: Consider integrating Intrusion Detection Systems (IDS) or Intrusion Prevention Systems (IPS) with the firewall to detect and automatically respond to malicious activity.
* **Security Benefit:**
    * Creates a barrier against unauthorized network access.
    * Prevents or mitigates various attacks, such as malware infections, data breaches, and denial-of-service (DoS) attacks.
    * Controls the flow of data, reducing the risk of data exfiltration.

**Multi-Factor Authentication (MFA) Enforcement:**

* **The Problem:**
    * The absence of MFA means that if an attacker obtains a user's password (through phishing, brute-force, or other means), they can easily gain full access to the account.
* **The Solution:**
    * Implement MFA for all user accounts, especially administrative accounts, and any accounts with access to sensitive data.
    * MFA methods can include:
        * Authenticator apps (e.g., Google Authenticator, Authy)
        * SMS-based one-time codes (less secure but better than nothing)
        * Hardware security keys (e.g., YubiKey)
    * Educate users on the importance of MFA and how to use it correctly.
* **Security Benefit:**
    * Adds an extra layer of security beyond passwords, making it significantly harder for attackers to gain unauthorized access even if they have a valid password.
    * Provides strong protection against phishing attacks and credential theft.

By implementing these hardening measures, the social media organization can significantly improve its security posture, reduce the risk of future data breaches, and better protect its customers' personal information.
