## Email Servers 

Before launching a phishing campaign, configuring whitelisting on email servers is essential to ensure the emails are delivered successfully and not blocked or marked as spam. 

--- 

### Office365 

- To successfully whitelist emails for dPhish phishing simulations in Office 365, please follow the steps below. Ensure that you have security administrator privileges within the Microsoft Security Center before proceeding. 

    1. Sign in to the `Microsoft Security` Center using your security administrator credentials. 

    2. In the left sidebar menu, click on `Policies` & `rules`. 

    3. Navigate to `Threat policies` and select `Advanced delivery`. 

    4. Click on the `Phishing simulations tab`, then click `Edit`. 

    5. Under the `Sending IP` section, add the IP address associated with the phishing simulation. 

    7. In the `Domains` section, input the domain address used for the phishing campaign. 

    8. (Optional) To allow the phishing domains in the simulation URLs, use the wildcard syntax *.domain.com/* in the `Simulation URLs to allow` section. 

    9. Click `Save` to apply the changes and complete the whitelisting process. 

---

### Exchange Server 

1.  Open Exchange Admin Center (EAC) 

    **For Exchange* 2013/2016/2019**: 

    - Open your browser and navigate to the Exchange Admin Center (EAC). 

    - The URL for the EAC typically looks like https://<ExchangeServerFQDN>/ecp (replace <ExchangeServerFQDN> with your server’s Fully Qualified Domain Name). 

    - Log in using an admin account with the necessary privileges. 

2. Create a New Accepted Domain 

    - An `Accepted Domain` in Exchange refers to a domain for which the Exchange server will accept and process emails. 

3. **Navigate to Mail Flow**: 

    - In the left-hand pane of the EAC, click on `Mail Flow`. 

4. **Create a New Accepted Domain**: 

    - Under `Mail Flow`, select `Accepted Domains`. 

    - Click on the + icon to create a new accepted domain. 

5. **Add the Trusted Domain**: 

    - In the New Accepted Domain wizard, fill out the following: 

        **Name**: A display name for the domain (e.g., "Trusted Domain"). 

        **Accepted Domain**: The fully qualified domain name (FQDN) of the trusted domain (e.g., trustedcompany.com). 

        **Type**: Choose `Authoritative Domain` if emails are hosted and managed by your Exchange server, or Internal Relay Domain if emails for the domain are routed to another server for delivery. 

6. Click `Save`. 

---

### Google Workspace 

1. Log in to the Google Admin Console 

2. Visit the Google Admin Console and log in using your administrator credentials. 

3. Navigate to Gmail Settings 

4. Once logged in, click on the Apps section from the main console screen. 

5. Choose Google Workspace > Gmail. 

6. Configure the Spam and Allow List Settings 

7. Under Gmail Settings, click on Spam, Phishing, and Malware. This section allows you to manage filters for inbound email and configure trusted senders. 

8. Whitelist Trusted Domains 

9. Scroll down to the Approved Senders section (this may vary based on your version of Google Workspace). 

10. Here, you can enter the domains you want to trust.To allow emails from a specific domain, enter the domain name (e.g., @trusted-domain.com). This will whitelist all emails coming from this domain. 

--- 

### Postfix 

To add a trusted domain or URL in Postfix, you would typically modify the configuration to whitelist specific domains or IP addresses, preventing them from being marked as spam or being blocked. 

1. **Log in to Your Server**: 

    - SSH into your server where Postfix is installed. 

2. **Edit the Postfix Configuration**: 

    - Open the main Postfix configuration file: sudo nano /etc/postfix/main.cf 

3. **Add Trusted Domains to smtpd_sender_restrictions**: 

    - Add the trusted domain to the smtpd_sender_restrictions line. This tells Postfix to allow email from the trusted domain. 

4. smtpd_sender_restrictions = check_sender_access hash:/etc/postfix/sender_access, permit_mynetworks, reject_unauth_pipelining 

    - Create or edit the /etc/postfix/sender_access file: sudo nano /etc/postfix/sender_access 
 
    - Add the trusted domain or email address in the file (for example, trusted.com): trusted.com OK 

5. **Create Hash Database for sender_access**: 

    - After editing the file, generate the hash database: sudo postmap /etc/postfix/sender_access 

6. **Restart Postfix**: 

    - Apply the changes by restarting the Postfix service: sudo systemctl restart postfix 

---

### FireEye Cloud Mail Gateway 

1. **Log in to the FireEye Cloud Console**: 

    - Open your web browser and go to the FireEye Cloud login page (typically https://cloud.fireeye.com). 

    - Enter your credentials to access the `FireEye Cloud Console`. 

2. **Access the Email Security Configuration**: 

    - Once logged in, navigate to the `Email Security` section. This is where you can manage all email security-related configurations, including policies for filtering, spam, malware, and more. 

    - In some environments, this might be listed under Mail Gateway or `Trellix Email Security`. 

3. **Navigate to the Whitelist or Allow List Section**: 

    - Look for a section related to Policies, Anti-Spam, or Allow List. 

    - This section is where you can manage exceptions for trusted domains or email addresses, ensuring they are not flagged as spam or malicious. 

4. **Add the Domain or Email Address to the Whitelist**: 

    - In the `Allow List` section, you’ll need to add either: 

        1. **Email addresses** (e.g., user@example.com) 

        2. **Domains** (e.g., example.com) 

    - For example, if you want to whitelist emails from the domain trusted.com, you would enter @trusted.com to allow all emails from that domain. 

5. **Configure the Action**: 

    - Ensure the action is set to `Allow` or `Bypass Spam Filtering` for the added email addresses or domains. This ensures that emails from these sources will not be subject to spam or threat filtering. 

    - You may also configure additional settings like the `filtering level` (if any) for the whitelisted emails. 

6. **Save and Apply the Changes**: 

    - After adding the trusted email addresses or domains to the whitelist, `save` the changes. 

    - Depending on your system setup, you might need to `apply` the changes or wait for them to take effect. 