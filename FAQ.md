# Frequently Asked Questions (FAQ)

- [Why was my phishing email not delivered?](#why-was-my-phishing-email-not-delivered)
- [CSS issue in templates](#css-issue-in-templates)
- [Is the tracker host empty?](#is-the-tracker-host-empty)
- [Couldn’t find the Announcement template or the Announcement page?](#couldnt-find-the-announcement-template-or-the-announcement-page)
- [Redirect to Dashboard when clicking on any tap](#redirect-to-dashboard-when-clicking-on-any-tap)



## Why was my phishing email not delivered?

We can solve it through `4 steps`:

- Whitelist
- Safe Sender
- Check our mail senders (if it’s working, login and check)
- Contact Cybersecurity Team to check gateway and logs

---

## CSS issue in templates

It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like).

---

# Image issues in templates

---

# Course Assign Notification Issue

---

# Credentials not working for LMS 

---

## User accounts Created but credentials emails not delivered 

When convert targets to drill user, user account Created but credentials emails not delivered.

---

# Phishing email arrive in Junk mail

---

# Need to delete the data for one or more target from campaign 

---

## Using `.live` & `.com` as Notification Senders for large or small numbers of employes

`.com` domains limited to a specific number of emails / per day,

While `.live` is not limited.

We can solve it through:

- `notifications@dphish.live` = Large Number of Employes (5000 for example)

- `notifications@dphish.com` = Small Number of Employes

---

## There are 2 stores:

1. Egypt Store
2. KSA Store

- Egypt Store = https://demoksa.dphish.live/ 
- KSA Store = https://store.dphish.live/

We can solve it through:

- **Egypt** Store = `Demoksa`

- **KSA** Store = `Store`

---

## notification@dphish.com

`.com` Notification Sender’s Credentials

We can solve it through:

- `TLS`: True
- `Password`: *********
- `Port`: 587
- `Host`: smtp.office365.com
- `From`: Cybersecuiry Notification <notification@dphish.com>

---

## notification@dphish.live

`.live` Notification Sender’s Credentials

We can solve it through:

- `TLS`: True

- `Password`: *********

- `Port`: 587

- `Host`: mail.dphish.live

- `From`: dPhish Notification <notifications@dphish.live>

---

## Difference between Support Mobile & Support Phone (in Settings > LMS)

We can solve it through:

- `Support Mobile` appears on the `footer of the LMS`.

- `Support Phone` appears on `Cyber_Awareness_Email`.

---

## Drill users don't receive otp 

when drill users login to platform, they didn't receive otp

We can solve it through:

- They should do a whitelist for notification sender.

Another solution:

- The customer can put his own notification sender.

---

## The fast login button in the email for the assign course isn't working and it's showing an error with the drill user.

We can solve it through:

- First, make sure the email was sent within a week; if it's been more than a week, it’s expired.

- If it's less than a week, press `Ctrl+Shift+R` to clear the cache on the client’s side.

Another solution:

- Send the drill user the link to their platform and tell them to forget the password.

---

## The email is flagged despite being whitelisted & trusted.

When Google blacklists a tracker, the email is flagged, even if it has been whitelisted.

We can solve it through:

- Changing the tracker with a new one will solve it.

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

## Configuring the Client Notification Sender.

**Issue**:
The `Notification Sender` is not functioning correctly and fails to send emails.

**Solution**:
1. Identify the Email Service Provider:
    - Determine if the service is using `Exchange` or `Office 365 (O365)`.
    - Navigate to `Settings` → `Platform` → `Email Service`, and enter the appropriate provider details.

2. Enable Custom Notification Sender:
    - Go to `Settings` → `Notification Sender` and ensure the `Custom Notification Sender` is enabled.

3. Adjust Sender Port (if using Exchange):
    - Set the `Sender Port` to `443`.

4. Final Step (if the issue persists):
    - Configure the `Sender From Email` only and retry sending notifications.