## Web Proxy (Web Filter)

Before launching a phishing campaign, configuring the web proxy (web filtering) is essential to ensure the campaign links function correctly and are not blocked.  

--- 

### Defender for Office 365

1. **Login to Microsoft 365 Defender Portal**:  

2. Navigate to the **Microsoft 365 Defender Portal**: https://security.microsoft.com  

3. Log in with your **admin credentials**.  

4. **Access the Security & Compliance Center**:  

5. In the Defender portal, go to the `Security` & `Compliance Center`.  

6. If you're using `Microsoft 365 Defender`, go to the `Threat Management` section.  

7. **Configure Safe Links Policies**:  

8. In the `Microsoft Defender portal`, select `Threat management` > `Policy` > `Safe Links`.  

9. If you don’t already have a Safe Links policy, create one by clicking + `Create Policy`.  

10. **Create or Edit Safe Links Policy**:  

11. If you're creating a new policy, provide a name and description for your policy.  

12. If you already have an existing Safe Links policy, click to `edit` that policy.  

13. **Add Trusted Domains**:  

14. In the policy editor, go to the `Advanced Settings` section.  

15. Look for the setting that allows you to configure Trusted Domains or `Do not rewrite the URLs in messages from these domains`.  

16. Add the domain(s) you want to trust (e.g., trusted-domain.com) into this list. This will ensure that emails from these domains will not have their links `rewritten` by Microsoft Defender for Office 365. 

---

### Fortinet  

1. Log in to FortiGate Web Interface 

2. Open a browser and navigate to the FortiGate web interface (usually https://<your-fortigate-ip>). 

3. Enter your admin credentials. 

4. Create or Edit a Web Filter Profile 

5. Go to Security Profiles > Web Filter. 

6. If you don’t have an existing Web Filter Profile, click Create New. If you already have one, select it to edit. 

7. Under the Web Filter Profile settings, find the URL Filter or Exempt URL section. 

8. Add the domains or URLs you want to whitelist to ensure they bypass filtering. For example: 

9. For a domain: trusted-domain.com 

10. Set the action to Allow for the whitelisted entries. 

11. Save and Apply the Web Filter Profile 

12. After adding the necessary domains or URLs to the whitelist, click OK or Save. 

13. Go to Policy & Objects > IPv4 Policy or IPv6 Policy. 

14. Select the Web Filter Profile you just updated and apply it to the appropriate Firewall Policy. 

---

### TrendMicro 

1. **Log in to Trend Micro Cloud App Security Console**: 

    - Open your browser and navigate to the `Trend Micro Cloud App Security Console`. 

    - Log in with your administrator credentials. 

2. **Navigate to the URL Filtering Section**: 

    - Once logged in, go to `Settings` or `Policies` in the main menu. 

    - In the settings menu, locate the `URL Filtering` or `Web Filtering section` (it may vary depending on the version). 

3. **Add Trusted Domains or URLs to the Allow List**: 

    - Look for the `Allow List` or `Exclusions` section. 

    - Here you can add domains or URLs that should be trusted and not filtered. 

    - To add a domain, click on `Add Domain` or `Add URL`. Enter the domain or URL you want to whitelist. For example, trusted.com or https://trusted-domain.com. 

    - You can use wildcard entries (e.g., *.trusted.com) to allow all subdomains. 

4. **Apply the Changes**: 

    - Once you have added the domains or URLs to the whitelist, click `Save` or `Apply` to update the settings. 

---

### SonicWall 

1. **Log in to the SonicWall Management Console**: 

    - Open your web browser and go to your SonicWall device's management IP address (e.g., https://192.168.1.1). 

    - Log in with your administrator credentials. 

2. **Navigate to the Content Filtering Section**: 

    - In the SonicWall interface, go to Security Services. 

    - Under the Content Filter tab, select Content Filtering Service (CFS). 

3. **Add Trusted Domains to the URL Filtering List**: 

    - In the CFS section, you can configure a whitelist to allow specific domains or URLs. 

    - Scroll to the Exemptions or Allow List section (depending on the SonicWall version). 

    - Click on Add to include a trusted domain or URL. For example, to trust trusted.com, you would enter trusted.com or *.trusted.com to allow all subdomains. 

4. **Specify URL Patterns or Domains**: 

    - You can enter specific URLs or domains to allow. For example: 

        1. trusted.com (for the main domain). 

        2. *.trusted.com (for all subdomains). 

        3. https://trusted.com/specific-page (for a specific page). 

5. **Save the Changes**: 

    - Once you’ve added the domains or URLs to the Allow List, save the settings. 

    - Make sure the changes are applied to the relevant user groups or policies. 

---

### AppRiver Secure Web Gateway  

1. **Log in to the AppRiver Control Panel**: 

    - Open a browser and go to the `AppRiver Portal`: https://portal.appriver.com. 

    - Log in using your administrator credentials. 

2. **Navigate to the Secure Web Gateway Section**: 

    - Go to the `Secure Web Gateway (SWG)` section within the control panel. 

3. **Locate the URL Filtering Settings**: 

    - Look for `URL Filtering` or `Web Filtering` settings. 

    - These settings allow you to configure the categories of sites that are allowed or blocked. 

4. **Add Trusted Domains or URLs to the Allow List**: 

    - In the `Allow List` or `Whitelist` section, add the trusted domain or URL you wish to allow. 

    - For example, enter trusted-domain.com to allow access to this domain without filtering. 

    - You can also add specific URLs (e.g., https://trusted-domain.com/allow-page) if needed. 

5. **Save the Configuration**: 

    - Once you have added the trusted domains or URLs, click `Save` or `Apply` to update your settings. 

---

### Forcepoint Web Security 

1. **Log in to the Forcepoint Admin Console**: 

    - Open a web browser and go to the Forcepoint Web Security login page. 

    - Enter your admin credentials to access the administrative console. 

2. **Navigate to the Policy Section**: 

    - In the Forcepoint Admin Console, go to the `Policies` tab, where you can configure the various filtering rules. 

    - In some versions, this may be under `Web Security` > `URL Filtering` or `Web Filter Policies`. 

3. **Configure URL Filtering Settings**: 

    - Under the Policy section, find the `URL Filtering` settings. Here, you will be able to configure allow lists and exceptions. 

    - Alternatively, look for `Exclusions` or Allow List in the menu options. 

4. **Add Trusted Domains to the Allow List**: 

    - In the Allow List (or Exclusion List) section, click Add to enter a trusted domain. 

    - Enter the full domain or URL you want to trust (e.g., trusted-domain.com). 

    - If you want to allow an entire domain, just specify the domain name (e.g., trusted-domain.com), or you can add specific subdomains (e.g., sub.trusted-domain.com). 

5. **Apply the Action to the Trusted Domain**: 

    - Set the action for the domain to Allow or Bypass, which will instruct Forcepoint to bypass filtering policies for this domain. 

    - Make sure to select the appropriate action that ensures the trusted domain is allowed without being subject to filtering. 

6. **Save and Apply Changes**: 

    - After adding the trusted domain, click `Save` or `Apply` to commit the changes and ensure they are active. 

---

### Zscaler Web Filter

1. **Log in to Zscaler Admin Portal**: 

    - Open a web browser and navigate to the Zscaler Admin Portal. 

    - Log in with your admin credentials. 

2. **Navigate to Web Filtering Policies**: 

    - Once logged in, in the Zscaler Admin Dashboard, go to the `Policy` tab. 

    - Under Policy, select `Web Access Control` or `URL Filtering` (the exact name may vary depending on your version). 

3. **Access the `Allow` or `Whitelist` Settings**: 

    - Find the option for `URL Categories` or Allow `List/Whitelist`. 

    - Zscaler allows you to create exceptions based on domains, URLs, or specific categories, so you can create an allow list for trusted domains. 

4. **Add Trusted Domain to the Allow List**: 

    - In the Allow List section, click Add or Add URL to include a new domain. 

    - Enter the domain you want to trust (e.g., trusted-domain.com). 

    - Zscaler allows you to add full domains (e.g., trusted-domain.com) or specific subdomains (e.g., sub.trusted-domain.com). 

5. **Configure Action to Bypass Filtering**: 

    - After adding the domain to the allow list, configure the action for this domain. The typical action will be Allow, meaning traffic from this domain will bypass content filtering, URL categorization, and other security features. 

6. **Save and Apply Changes**: 

    - After adding the trusted domains, click `Save` or `Apply` to ensure the changes are active. 

---

### VIPRE Web Filtering 

1. **Log in to the VIPRE Management Console**: 

    - Open your browser and log in to the VIPRE Management Console using your administrator credentials. 

2. **Navigate to the Web Filtering Section**: 

    - Once logged in, go to the `Web Filtering` or `Content Filtering` section. 

3. **Access the Allow List or Exemption Settings**: 

    - Look for the section where you can add `websites` or `URLs` to the Allow List (sometimes referred to as an Exemption List). 

    - This is where you specify trusted `domains` or `URLs` that should bypass the filtering. 

4. **Add Trusted Domains or URLs**: 

    - Click on `Add URL` or `Add Domain` to enter the trusted domains or URLs. 

    - For a domain, enter trusted-domain.com to allow all traffic from that domain. 

    - For a specific URL, you can add https://trusted-domain.com/specific-page to allow just that page. 

    - You can also use wildcards, e.g., *.trusted-domain.com to allow all subdomains of a domain. 

5. **Save the Configuration**: 

    - After entering the trusted domains or URLs, click `Save` or `Apply` to save your changes. 

---

### EdgeWave

1.   **Log in to the EdgeWave Web Filter Management Console**: 

    - Open your browser and go to the EdgeWave Web Filter Management Console. 

    - Enter your administrator credentials to log in. 

2. **Navigate to the URL Filtering Settings**: 

    - Go to the `Policy` or `Settings` section, then find `URL Filtering` or `Web Filtering` options. 

    - Look for the area where you can manage Allow List or Exemptions. 

3. **Add Trusted URLs or Domains**: 

    - In the Allow List section, add the trusted `domain` or `URL` you want to whitelist. 

    - For example: 

        - Add trusted.com to allow all URLs under that domain. 

        - Add specific URLs like https://trusted.com/special-page if you want to whitelist a specific page. 

    - If you need to use wildcards, you can specify *.trusted.com to cover all subdomains of that domain. 

4. **Save the Configuration**: 

    - After entering the trusted domain or URL, save the changes by clicking `Save` or `Apply`. 

---

### Cisco Umbrella 

1. **Log in to the Cisco Umbrella Dashboard**: 

    - Access the Cisco Umbrella Admin Console by going to https://dashboard.umbrella.com and logging in. 

2. **Go to Policies**: 

    - From the Dashboard, navigate to `Policies` > `Security Settings`. 

    - Select the appropriate policy for your `network` or `group`. 

3. **Configure URL Filtering**: 

    - In the Security Settings section, locate `URL Filtering` or `Categories`. 

    - Cisco Umbrella categorizes websites into predefined categories (e.g., social media, malware, etc.). To allow a specific URL, you’ll need to add it to the allowed list for URLs. 

4. **Add Trusted URLs to the Allow List**: 

    - Under the Allow List, click on Add `URL` or Add to `Whitelist`. 

    - Enter the exact `URL` or `domain` (e.g., https://trusted-url.com). 

    - Ensure that the URL is set to `Allow` or `Bypass Filtering`. 

5. **Save and Apply**: 

    - After adding the trusted URLs, click `Save` or `Apply` 

---

### Mimecast 

1. **Log in to the Mimecast Admin Console**: 

    - Open your browser and log in to the Mimecast Admin Console using your admin credentials. 

2. **Go to Administration Settings**: 

    - In the Mimecast Admin Console, go to `Administration` > `Gateway` > `Policies`. 

3. **Navigate to URL Filtering**: 

    - Select URL Filtering (or Attachment Management if it pertains to attachments with links). 

    - Go to the `Allow` List or `Trusted` URL List. 

4. **Add Trusted URLs**: 

    - Click New to add a trusted URL. 

    - Enter the URL (e.g., https://trusted-url.com). 

5. **Configure Settings**: 

    - You can specify additional details such as whether the URL applies to certain policies (e.g., email scanning, spam filtering) or if it should bypass all security checks. 

    - Ensure that the URL is not flagged as malicious by Mimecast’s URL filtering system. 

6. **Save and Apply**:  

    - After adding the trusted URLs, click Save to apply the changes  

---

### FireEye Cloud Web Filter

1. **Log in to the FireEye Cloud Console**: 

    - Go to the FireEye Cloud URL (typically https://cloud.fireeye.com) and log in with your admin credentials. 

2. **Access Web Security Configuration**: 

    - Once logged in, navigate to the `Web Security` section. This is where you can configure policies, including URL filtering and threat protection for web traffic. 

    - In some cases, this might be referred to as `Cloud Threat Detection` or `Web Filtering` depending on your FireEye product configuration. 

3. **Find the Whitelist Section**: 

    - Look for sections such as `URL Filtering`, `Policy`, or `Allow List`. The option to whitelist domains or IPs is typically located under URL filtering or security policy management. 

    - In some interfaces, you might see options like `Custom Policies` or `Exclusions,` where you can define exceptions for domains and IPs. 

4. **Add Domains, URLs, or IPs to the Whitelist**: 

    - In the whitelist or exclusion section, you can `add URLs`, `domains`, or `IP addresses` that you want to allow. 

    - **For URL Whitelisting**: 

        - Enter the `full URL` (e.g., https://example.com) or a domain (e.g., example.com). 

    - **For IP Whitelisting**: 

        - Enter the `IP address` (e.g., 192.168.1.1) or a range of IP addresses if you want to allow traffic from certain sources. 

    - There might be specific fields to add `IP` or `domain` exceptions based on your needs. 

5. **Configure the Action**: 

    - After adding the URLs, domains, or IPs, ensure that the action is set to "Allow" or "Whitelisted." 

    - This will ensure that traffic to/from these sources bypasses any `filtering` or `blocking` that is typically applied by the FireEye Web Filter. 

6. **Save and Apply the Changes**: 

    - After adding the `domains` or `IPs` to the whitelist, `save` the changes. 

    - Depending on your configuration, you might need to `apply the policy` or `refresh` the system for the changes to take effect. 

---

### How to Whitelist Using the dphish Phishing Simulations Feature in Office 365

To successfully whitelist emails for dphish phishing simulations in Office 365, please follow  

the steps below. Ensure that you have security administrator privileges within the  

Microsoft Security Center before proceeding. 

1. Sign in to the Microsoft Security Center using your security administrator credentials. 

2. In the left sidebar menu, click on Policies & rules. 

3. Navigate to Threat policies and select Advanced delivery. 

4. Click on the Phishing simulations tab, then click Edit. 

5. Under the Sending IP section, add the IP address associated with the phishing simulation. 

6. In the Domains section, input the domain address used for the phishing campaign. 

7. (Optional) To allow the phishing domains in the simulation URLs, use the wildcard syntax  

*.domain.com/* in the Simulation URLs to allow section. 

8. Click Save to apply the changes and complete the whitelisting process. 


---

### Add Domains to Outlook Safe Sender Lists

To add your domains to the Outlook Safe Sender lists of all end users, it is necessary to run a  

PowerShell script. This step should be repeated whenever new users are added or before running a simulated phishing campaign. 

---

### Prerequisites

- Administrative Privileges: PowerShell must be run with administrative rights. 

- An Exchange Administrator Role and valid credentials to access the Office 365 account. 

- Exchange Online PowerShell Module: Ensure that the Exchange Online PowerShell module is  

installed on the system. 

---

### Step-by-Step Guide

1. **How to Install Exchange Online PowerShell Module**: 

    - Open PowerShell as Administrator. 

    - Run the following command to install the Exchange Online Management module: 

        - Install-Module -Name ExchangeOnlineManagement 

2. **Open PowerShell in Single Threaded Apartment (STA) Mode**: 

    - Open a new PowerShell session in STA mode using the command below: 

        - powershell.exe -STA 

3. **Import the Exchange Online Module and Connect to Exchange Online**: 

    - Import the Exchange Online Management module: 

        - Import-Module ExchangeOnlineManagement 

    - Connect to your Exchange Online account by providing your credentials: 

        - Connect-ExchangeOnline -UserPrincipalName your_email@domain.com 

4. **Add Domains to Safe Sender List**: 

    -  To add your domains to the Outlook Safe Sender list, use the following command: 

        - $All = Get-Mailbox -RecipientTypeDetails UserMailbox -ResultSize Unlimited; $All | foreach {SetMailboxJunkEmailConfiguration $_.Name -TrustedSendersAndDomains @{Add="mail.alexandriadigital.digital"}} 

---

### Important Notes: 

- You need to run this script each time you add new users to ensure the domains are added to  

their Safe Sender lists. 

- It is recommended to execute this script before launching any simulated phishing campaign. 

- If the Get-Mailbox command does not return the expected results, it may be necessary to use  

the Get-EXOMailbox command as an alternative. 

---

### Step-by-Step Validation Process: 

To ensure proper validation of the following steps, it is recommended to use an alternative  

account for testing. 

---

### New Outlook/Browser Outlook: 

1. **Access Outlook Settings**: 

    - Open Outlook and click on the settings icon 

2. **Navigate to Mail**: 

    - From the settings menu, select Mail to open the email settings options. 

3. **Access Junk Email Settings**: 

    - In the left-hand pane, click on Junk email. 

4. **Review Safe Senders and Domains**: 

    - Scroll down to the `Safe senders` and `domains section`. Review the listed entries to  

5. **confirm the correct configuratio** 