## Add Domains to Outlook Safe Sender Lists

This step is essential to ensure smooth communication and functionality for platform's email services.  

By adding our domain to the trusted senders list, emails from your platform are automatically marked as safe. This allows images, including tracking components like open rate pixels, to load without requiring user intervention. 

By marking domain as trusted, emails are delivered directly to users' inboxes instead of being sent to the junk folder. 

With domain added as a trusted sender, images are displayed automatically, enhancing the user experience, and improving the visibility of your platform's branding and content. 

To add your domains to the Outlook Safe Sender lists of all end users, it is necessary to run a PowerShell script. This step should be repeated whenever new users are added or before running a simulated phishing campaign.  

---

### Prerequisites

- **Administrative Privileges**: PowerShell must be run with administrative rights. 

- **An Exchange Administrator Role** and valid credentials to access the Office 365 account. 

- **Exchange Online PowerShell Module**: Ensure that the Exchange Online PowerShell module is  

installed on the system. 

---

### Step-by-Step Guide

1. **How to Install Exchange Online PowerShell Module**: 

    - Open PowerShell as Administrator. 

    - Run the following command to install the Exchange Online Management module: 

        - **Install-Module -Name ExchangeOnlineManagement **

2. **Open PowerShell in Single Threaded Apartment (STA) Mode**: 

    - Open a new PowerShell session in STA mode using the command below: 

        - **powershell.exe -STA**

3. **Import the Exchange Online Module and Connect to Exchange Online**: 

    - Import the Exchange Online Management module: 

        - **Import-Module ExchangeOnlineManagement**

    - Connect to your Exchange Online account by providing your credentials: 

        - **Connect-ExchangeOnline -UserPrincipalName your_email@domain.com**

4. **Add Domains to Safe Sender List**: 

    -  To add your domains to the Outlook Safe Sender list, use the following command: 
        
        - **$All = Get-Mailbox -RecipientTypeDetails UserMailbox -ResultSize Unlimited
            $All | ForEach-Object {
            Set-MailboxJunkEmailConfiguration -Identity $_.Name -TrustedSendersAndDomains @{Add="mail.alexandriadigital.digital"}}**

---

### Important Notes: 

- You need to run this script each time you add new users to ensure the domains are added to their Safe Sender lists. 

- It is recommended to execute this script before launching any simulated phishing campaign. 

- If the `Get-Mailbox` command does not return the expected results, it may be necessary to use the `Get-EXOMailbox` command as an alternative. 

---

### Step-by-Step Validation Process: 

To ensure proper validation of the following steps, it is recommended to use an alternative account for testing.

---

### New Outlook/Browser Outlook: 

1. **Access Outlook Settings**: 

    - Open Outlook and click on the `settings` icon.

2. **Navigate to Mail**: 

    - From the settings menu, select `Mail` to open the email settings options. 

3. **Access Junk Email Settings**: 

    - In the left-hand pane, click on `Junk email`. 

4. **Review Safe Senders and Domains**: 

    - Scroll down to the `Safe senders and domains` section. Review the listed entries to confirm the correct configuration.

![WhiteListing safe sender and domain!](../../assets/whiteListing/safe_sender_domain.png "WhiteListing safe sender and domain")

---

### Old Outlook (desktop):

1. **Open Outlook**: 

    - Launch the `Outlook` desktop application.

2. **Right-Click on Any Email**: 

    - Right-click on any email in your inbox to access additional options.

3. **Select Junk**: 

    - From the context menu, choose `Junk`.

4. **Choose Junk Email Options**: 

    - Click on `Junk Email Options` to access the configuration settings.

5. **Navigate to Safe Sender**:

    - In the `Junk Email Options` window, select the `Safe Senders` tab to manage the list of safe senders and domains.

![WhiteListing safe sender junk email!](../../assets/whiteListing/safe_sender_junk.png "WhiteListing Safe Sender Junk")


![WhiteListing safe sender!](../../assets/whiteListing/safe_sender.png "WhiteListing Safe Sender")