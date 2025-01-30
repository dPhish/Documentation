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