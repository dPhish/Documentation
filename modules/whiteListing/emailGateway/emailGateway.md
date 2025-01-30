## Email Gateway 

Before launching a phishing campaign, it is crucial to configure the whitelisting feature on the email gateway to ensure smooth delivery of campaign emails. 

--- 

### Defender for Office 365 

- `Microsoft Defender for Office 365` is a cloud-based security solution designed to protect your organization against advanced threats targeting email and collaboration tools, such as phishing, business email compromise, and malware attacks. It offers comprehensive protection by integrating seamlessly with Microsoft 365 services, providing features like Safe Links, Safe Attachments, and anti-phishing policies to safeguard users. 

    1. Login to the Microsoft 365 Defender Portal as described above.  

    2. Navigate to Anti-Phishing Policies:  

    3. In the Microsoft Defender portal, go to `Threat management` > `Policy` > `Anti-Phishing`.  

    4. Create or Edit Anti-Phishing Policy:  

    5. If creating a new policy, click + Create Policy and follow the wizard.  

    6. If editing an existing policy, select the policy and click Edit.  

    7. Add Trusted Domains (Senders):  

    8. In the policy editor, you’ll see a section for Domain/Email Sender Trust.  

    9.Here, you can add trusted senders or trusted domains to ensure emails from those domains bypass anti-phishing protections.  

    10. Add the domain you wish to trust (e.g., trusted-domain.com).  

    11. Save Changes:  

    12. After adding trusted domains, click Save to apply the new configuration.  

---

### Microsoft Exchange Server 

1. Open Exchange Admin Center (EAC): 

2. Go to `Servers` > `Accepted Domains`. 

3. Click on + Add a domain. 

4. Add the Trusted Domain: 

5. Choose whether this domain will be Authoritative (your Exchange server is responsible for this domain) or Internal Relay (forwarding to another mail server). 

6. Enter the domain name (example.com). 

--- 

### FortiMail 

- `FortiMail` is a secure email gateway that provides a range of email filtering services, including spam filtering, virus scanning, and advanced email protection. It can be used as part of an organization’s email infrastructure, often placed between the internal mail server (like Microsoft Exchange) and the internet to protect against threats.	 

1. First Log in to FortiMail Web Interface 

    - Open your web browser and navigate to your FortiMail device's web interface (usually https://<your-fortimail-ip>). 

    - Log in with your admin credentials.  

2. Whitelist a Domain or IP Address for users over Fortimail 

- **Whitelist a Sender or Domain in FortiMail**

3. To whitelist a sender or domain in FortiMail, follow these steps: 

    - Go to Anti-Spam Profile Settings: 

    - Navigate to Profile > Anti-Spam. 

    - Look for a section that allows you to configure the Sender Whitelist or Domain Whitelist. 

    - Add a Sender or Domain to the Whitelist: 

4. For whitelisting a sender's email address (support@domain.com), enter the full email address in the appropriate field. 

5. For whitelisting a domain (domain.com) 

6. Save the Configuration: 

7. After adding the sender or domain to the whitelist, click OK or Save to apply the changes. 

8. Apply to Anti-Spam Policies: 

    - Ensure the updated Anti-Spam Profile is applied to the relevant incoming or outgoing mail policies. 

- **Whitelist an IP Address in FortiMail** 

1. To whitelist a sending server's IP address: 

2. Go to Anti-Spam Settings: 

3. Navigate to Profile > Anti-Spam > IP Address Whitelist. 

4. Add the trusted IP address (192.168.1.100). 

5. Save the Configuration: 

6. Save your changes and ensure they are applied to your incoming or outgoing mail policies. 

--- 

### Barracuda 

- The `Barracuda Email Security Gateway (ESG)` is a powerful email security solution designed to protect organizations from a wide range of email-borne threats. It offers comprehensive protection against spam, viruses, malware, phishing, and other email-based attacks, ensuring that your email infrastructure remains secure. 

    1. Log into the Barracuda Web Interface: 

    2. Open a web browser and go to the Barracuda Email Security Gateway login page (typically https://<your_barracuda_device_IP>). 

    3. Log in with your admin credentials. 

    4. Navigate to the `Email Security` section: 

    5. Once logged in, you'll be on the Barracuda Admin Dashboard. 

    6. In the left-hand navigation pane, select Mail Policies. 

    7. Go to the `Whitelist` or `Allowed Senders` Section: 

    8. In the Mail Policies tab, go to the Block/Accept section. 

    9. Here you will find the Allow List (or Whitelist) options, which allow you to add trusted domains or senders. 

    10. Add Trusted Domains: 

    11. In the Allow List section, click the Add button to add a new trusted domain. 

    12. You can either add individual email addresses or entire domains. 

    13. To add a domain, enter the domain name (e.g., trusted-domain.com) in the input field. This will ensure that all emails from this domain are allowed through without being blocked by the spam filter. 

    14. Save the Changes: 

    15. After entering the domain or sender, click Save to apply the changes. 

--- 

### Proofpoint  

- `Proofpoint Email Security` is a comprehensive and advanced solution designed to protect organizations against a wide range of email-based threats, including phishing, spam, malware, ransomware, and business email compromise (BEC). Proofpoint's email security services use a multi-layered approach to protect both inbound and outbound email communications, ensuring that both employees and organizational data remain safe from malicious attacks. 

    1. **Log into the Proofpoint Admin Console:** 

    2. Open a web browser and navigate to the Proofpoint `Email Protection` login page. 

    3. Log in with your `admin credentials`. 

    4. Access the `Admin Section`: 

    5. Once logged in, in the left-hand navigation pane, select `Policy`. 

    6. Under Policy, you will find various policy settings. Select `IP and Domain Allow Lists` or `Blocked Senders/Allow Senders` depending on your version of Proofpoint. 

    7. Adding a Trusted Domain: 

    8. In the `IP and Domain Allow Lists` section, click on `Add Domain`. 

    9. Enter the domain you wish to trust (e.g., trusted-domain.com). 

    10. This ensures that all emails from this domain will bypass the spam filtering and other security checks in Proofpoint. 

    11. **Adding a Trusted IP Address:**

    12. In the same section, you can add trusted `IP addresses`. 

    13. Click on Add IP Address. 

    14. Enter the IP address (e.g., 192.168.1.100) of the mail server that you want to trust. This ensures that emails from that IP address are not filtered. 

    15. **Apply and Save Changes:**

    16. After adding the domain and/or IP address, click `Save` or `Apply` to ensure the changes are saved. 

--- 

### Sophos  

- `Sophos Email Security` is an advanced email protection solution designed to safeguard businesses from a variety of email-based threats, including phishing, malware, ransomware, spam, and business email compromise (BEC). Sophos integrates AI-powered protection, real-time threat intelligence, and comprehensive filtering technologies to prevent attacks before they reach users’ inboxes. 

    1. Log in to Sophos Email Admin Console: 

    2. Navigate to the Sophos Email Admin Console. 

    3. Use your administrator credentials to log in. 

    4. Go to Anti-Spam or Policy Settings: 

    5. In the main console, go to the Policies section. 

    6. From here, you can access the Spam Protection or Email Filtering settings. 

    7. Create or Modify a Whitelist Policy: 

    8. Look for a policy or setting named Allow List, Whitelist, or Safe Senders. 

    9. If you're creating a new policy, select Create New Policy and choose Anti-Spam or Email Protection. 

    10. Under the Allow List section, you can add trusted domains or email addresses. 

    11. Add Trusted Domains to the Whitelist: 

    12. Enter the trusted domain (e.g., trusted.com) into the Allow List section. 

    13. You can add multiple domains or specific email addresses that you trust. 

    14. Save the Configuration: 

    15. After adding the domains or addresses to the whitelist, save the configuration. 

---

### Mimecast 

- `Mimecast` is a comprehensive cloud-based email security solution designed to protect organizations from a wide range of email-based threats, including phishing, malware, spam, ransomware, and business email compromise (BEC). Mimecast integrates email security, archiving, continuity, and compliance features into a unified platform, ensuring that email communications remain secure, accessible, and compliant. 

    1. Log in to the Mimecast Admin Console: 

    2. Open your web browser and navigate to the Mimecast Admin Console. 

    3. Enter your admin credentials to log in. 

    4. Go to the Administration Section: 

    5. In the top menu, select Administration > Gateway > Policies. 

    6. Navigate to Allow List: 

    7. Under Policies, look for Anti-Spam Policies. 

    8. Select Allow List (or Safe List depending on the version). 

    9. Add Trusted Domains: 

    10. Click New to add a trusted domain. 

    11. Enter the domain name you want to trust (e.g., trusted.com). 

    12. You can add multiple domains if needed. 

    13. Configure Settings: 

    14. In the domain entry, you can set specific conditions, such as whether the domain applies only to certain policies or global policies. 

    15. Choose the relevant policy that should apply to this domain (e.g., spam filtering). 

    16. Save the Configuration: 

    17. After adding the trusted domains, click Save to apply the changes. 

---

### Mcafee 

- `McAfee Email Security` is a robust, cloud-based solution designed to protect organizations from a wide range of email threats, including phishing, malware, spam, ransomware, and business email compromise (BEC). With advanced threat detection, data loss prevention (DLP), and advanced encryption capabilities, McAfee Email Security helps ensure that businesses can securely manage and protect their email communications. 

    1. Log in to the McAfee Email Protection Admin Console: 

    2. Navigate to the McAfee Email Protection Admin Console. 

    3. Use your administrator credentials to log in. 

    4. Navigate to Anti-Spam Settings: 

    5. In the main console, go to Policies or Protection Settings. 

    6. Select Anti-Spam or Email Filtering options. 

    7. Whitelisting Trusted Domains or IPs: 

    8. Look for an option called Allow List or Whitelist (this may vary slightly depending on your version). 

    9. Add the trusted domains or IP addresses to the whitelist. 

    10. Trusted Domain: Add a domain such as trusted.com to the allow list. 

    11. Trusted IP: Add the IP address of the trusted mail server (e.g., 192.168.1.1) to the allow list. 

    12. Save the Configuration: 

    13. After adding the trusted domains or IP addresses, make sure to save the changes. 

---

### ZIX 

1. Log in to the Zix Admin Console: 

2. Open your browser and log in to the Zix Admin Console using your administrator credentials. 

3. Go to the Filtering or Anti-Spam Settings: 

4. In the Admin Console, navigate to the Policy section. 

5. Under the Policies section, look for Spam Filtering, Email Protection, or similar options related to email filtering. 

6. Configure Safe Sender or Trusted Domains List: 

7. Find the Safe Sender List or Whitelisted Domains section. 

8. Here, you can add domains or email addresses you trust, so emails from these sources will bypass spam filters. 

9. Add a domain such as trusted.com or example.com. 

10. If you wish to add specific email addresses, you can add trusted@trusted.com as well. 

11. Save and Apply the Configuration: 

12. After adding the trusted domains or addresses, save the configuration. 

---

### Cisco Umbrella 

1. **Log in to the Cisco Umbrella Dashboard: **

    - Open your browser and navigate to the `Cisco Umbrella Admin Console` at https://dashboard.umbrella.com. 

    - Enter your admin credentials to log in. 

2. **Navigate to the Policies Section: **

    - In the left-hand menu, go to `Policies` > `Security Settings`. 

    - Select the Policy that is being applied to your network or group of users. If you haven’t created a policy, you can do so by clicking on `Create a New Policy`. 

3. **Configure the Domain Allow List: **

    - Under the `Policy` settings, look for the section labeled Block/Allow or Allow List. 

    - Here, you can add domains that you want to whitelist. These domains will not be subject to the usual Umbrella filtering rules. 

4. **Add Trusted Domains: **

    - Click `Add Domain` or `Add` to `Allow List`. 

    - Enter the domain name (e.g., trusted.com or example.com) and ensure it is set to "Allow" or "Bypass Filtering." 

5. **Save and Apply: **

    - Once you’ve added the trusted domains, click Save or Apply to implement the changes. 