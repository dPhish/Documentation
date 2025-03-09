## Why was my phishing email not delivered?

We can solve it through `4 steps`:

- Whitelist
- Safe Sender
- Check our mail senders (if it’s working, login and check)
- Contact Cybersecurity Team to check gateway and logs

---

 ## CSS issue in templates

**Issue**: 

Templates may experience CSS-related issues that affect their layout and visual appearance, causing inconsistencies in design or formatting. 

**Cause**: 

- CSS issues can arise due to: 

- Conflicting styles within the template. 

- Inherited styles from parent elements. 

- Missing or improperly linked CSS files. 

- Browser compatibility inconsistencies. 

**Solution**: 

1. **Inspect the Template**: 

    - Use browser developer tools to identify conflicting or missing CSS rules. 

2. **Validate CSS**: 

    - Ensure all CSS classes and IDs are correctly defined and applied. 

    - Check for syntax errors in the CSS code. 

3. **Resolve Conflicts**: 

    - Apply specific selectors to avoid style overrides. 

    - Use the !important declaration cautiously when needed. 

4. **Cross-Browser Testing**: 

    - Verify template rendering across different browsers to identify compatibility issues. 

5. **Clear Cache**: 

    - Perform a hard refresh (`Ctrl` + `Shift` + `R` or `Cmd` + `Shift` + `R`) to ensure the latest CSS changes are applied. 

If the issue persists, consider reviewing the template’s CSS structure or consulting with the development team for further troubleshooting. 

---

# Course Assign Notification Issue

**Issue**: 

When assigning a course to a user, the notification email is either not received or is delivered to the junk/spam folder. 

**Solution**: 

1. If the User Is Not Receiving the Email: 

    - Ensure the user has whitelisted the Notification Sender in their email settings to allow proper delivery. 

2. If the Email Is Delivered to the Junk/Spam Folder: 

    - Instruct the user to mark the Notification Sender as a Safe Sender to prevent future emails from being flagged as spam. 

Implementing these steps helps improve the deliverability of course assignment notifications. 

--- 

# LMS Credentials Not Working

**Issue**: 

Users are unable to log in to the `Learning Management System (LMS)` with their current credentials. 

**Solution**: 

1. `Click` on the `Forgot Password` link on the LMS login page. 

2. `Follow the instructions` to reset the password. 

3. `Log in` to the LMS using the new credentials after completing the password reset process. 

This process ensures secure account recovery and access to the LMS. 

---

## User Accounts Created but Credential Emails Not Delivered 

**Issue**: 

When converting targets to `Drill Users`, the user accounts are created, but the `credential emails` are not delivered. 

**Solution**: 

1. Navigate to `Settings` → `Platform`. 

2. Enable the option `Notify User on Creation`. 

This ensures that whenever a target is converted to a Drill User, the user will automatically receive their credential emails. s to drill user, user account Created but credentials emails not delivered.

---

# Phishing Simulation Email Delivered to Junk/Spam Folder

**Issue**: 

Phishing simulation emails are being delivered to the `junk/spam folder` instead of the inbox. 

**Solution**: 

- Ensure the `phishing simulation sender` is added to the recipient's `Safe Senders` list. 

- This helps improve email deliverability and ensures that future simulation emails are directed to the inbox

---

## Deleting Target Data from a Campaign 

**Issue**: 

There is a need to `delete data` for one or more targets within a campaign. 

**Solution**: 

1. To Delete Data for a Single Target: 

    - Navigate to the `Campaign`. 

    - Locate the specific `target` whose data you want to delete. 

    - `Delete` the target from the campaign to remove their associated data. 

2. To Delete Data for Multiple Targets: 

    - Repeat the process of `deleting individual targets` from the campaign `one by one`. 

3. To Clear All Trackers for All Targets in a Campaign: 

    - Go to `DO` → `Campaigns`. 

    - Click on the `three-dot menu` next to the desired campaign. 

    - Select `Clear Trackers` to remove all tracking data for all targets within the campaign. 

This process ensures that specific target data or all tracking data within a campaign can be efficiently managed. 

---


## Difference Between Support Mobile & Support Phone (in Settings > LMS) 

**Overview**: 

In `Settings` > `LMS`, you will find two distinct fields: `Support Mobile` and `Support Phone`. 

**Key Differences**: 

- **Support Mobile**: Displays in the `footer` of the LMS platform, providing users with quick access to mobile support contact information. 

- **Support Phone**: Appears in the `Cyber Awareness Email` communications, serving as the primary contact number for support-related inquiries. 

Ensure both fields are configured accurately to maintain consistent support information across the platform and emails. 

---

## Drill Users Not Receiving OTP 

**Issue**: 

When `Drill Users` attempt to log in to the platform, they do not receive the `One-Time Password (OTP)` required for authentication. 

**Solution**: 

1. Whitelist the Notification Sender: 

    - Ensure that the `Notification Sender` email address is whitelisted in the recipient's email server or spam filter settings. 

2. Use a Custom Notification Sender: 

    - If the issue persists, the customer can configure their own `Custom Notification Sender` through the platform settings. 

Proper configuration of the notification sender helps ensure reliable OTP delivery. 

---

## Fast Login Button Not Working for Assigned Course (Drill User) 

**Issue**: 

The `Fast Login` button in the assignment email is not functioning correctly, displaying an error when accessed by a `Drill User`. 

**Solution**: 

1. Verify Email Validity: 

    - Ensure the email was sent `within the past week`. Fast Login links expire after one week. 

2. Clear Browser Cache: 

    - If the email is still valid, instruct the user to perform a `hard refresh` by pressing `Ctrl` + `Shift` + `R` to clear the browser cache. 

3. Alternative Solution: 

    - If the issue persists, provide the Drill User with a direct link to the platform. 

    - Instruct them to use the `Forgot Password` option to reset their credentials and regain access. 

These steps help address common issues related to expired links and cached session data. 

---

## Email Flagged Despite Being Whitelisted and Trusted 

**Issue**: 

Emails are being flagged as suspicious or unsafe, or the tracker host is being blocked from the email, even though they have been whitelisted and marked as trusted. 

**Cause**: 

This issue can occur when `Google blacklists a tracker`, causing the email to be flagged regardless of its whitelist status. 

**Solution**: 

1. Edit the Campaign: 

    - `Replace the current tracker with a new one` within the campaign settings. 

    - This will resolve the issue and prevent the email from being flagged. 

Regularly monitoring tracker status can help identify such issues proactively. 

--- 

## Tracker Host Not Available During Campaign Setup.

**Problem**:
The tracker host field appears empty when creating a campaign and selecting a tracker host.

**Cause**:
This issue may occur if no tracking hosts have been added to the tenant.

**Solution**:
1. `Navigate to`: `Settings` → `Platform`.
2. `Add` the tracker hosts, ensuring they are separated by commas.
3. `Save` the updated settings.

If you do not have the required tracker hosts for the tenant, please contact the `Cybersecurity Department` to obtain them.

--- 

## Announcement Template or Page Not Found.

**Issue**:
The announcement template or announcement page is missing or not appearing during campaign creation.

**Solution**:
1. `Navigate to`: `Utilities` module.
2. `Locate` the desired template or page.
3. `Click on Actions` and select `Edit`.
4. `Ensure` the template or page is assigned to the `Announcement` category.

For the template or page to be available during the creation of an announcement campaign, it must be properly categorized under `Announcements`.

--- 

## Unexpected Redirection to Dashboard.

**Issue**:
Clicking on any tab redirects to the dashboard.

**Solution**:
Perform a `hard refresh` using one of the following methods:
- `Windows/Linux`: Press `Ctrl` + `Shift` + `R` or `Ctrl` + `F5`
- `Mac`: Press `Command` + `Shift` + `R`
If the issue persists, clear your browser cache and try again.

---

## Story Editing Error: Translations [object Object].

**Issue**:
When editing a story imported from the store, the error `translations: [object Object]` may appear.

**Solution**:
1. `Attempt to edit the story again`.
2. If the error persists, `delete the story` and manually `add it as a new story`.

This approach ensures proper formatting and avoids conflicts with imported data.

---

## Risk Score Not Updating After Campaign Execution.

**Issue**:
The risk score remains unchanged even after conducting a campaign.

**Solution**:
Ensure that `Drill Users` are present on the platform, as they are required for risk score calculations.

---

## Configuring the Client Notification Sender 

**Issue**: 

The Notification Sender is not functioning correctly and fails to send emails. 

**Solution**: 

1. Identify the Email Service Provider: 

    - Determine if the service is using `Exchange (EWS)` or `Office 365 (O365)`. 

    - Navigate to `Settings` → `Platform` → `Email Service`, and enter the appropriate provider details. 

2. Enable Custom Notification Sender: 

    - Go to `Settings` → `Notification Sender`. 

    - Ensure the Custom Notification Sender option is enabled. 

3. Configure Notification Sender Settings: 

    - Enter the following required details: 

        - **Sender User**: The email address or username used for authentication. 

        - **Sender Password**: The password associated with the sender’s account. 

        - **Sender Host**: The SMTP server address for the email service. 

        - **Sender Port**: The port used for sending emails: 

            - 443 if using Exchange (EWS) 

            - 587 if using Office 365 (O365) 

        - **Sender From**: The email address that will appear in the "From" field of sent notifications. 


4. Final Step (if the issue persists): 

    - Configure only the Sender From email and retry sending notifications. 

Properly configuring these settings ensures reliable email delivery from the notification sender. 
