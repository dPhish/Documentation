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

## CSS issue in templates

It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed to using 'Content here, content here', making it look like readable English. Many desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved over the years, sometimes by accident, sometimes on purpose (injected humour and the like).


## Is the tracker host empty?

This issue may be caused by the lack of tracking hosts added to the tenant. The solution to this issue is:

- Navigate to `Settings`, then select `Platform`. Add the tracker hosts seperated by commas, and ensure to save the new settings afterward.

- If you do not have the tracker hosts associated with the tenant, contact the cybersecurity department to obtain them.

## Couldn’t find the Announcement template or the Announcement page?

Navigate to the `Utilities` module, select the `template` or `page` you want to use, then click on Actions and choose `Edit`. Ensure that it is assigned to the `announcement category`.

To ensure that the template or page appears during the creation of the announcement campaign, it must be assigned to an announcement category

## Redirect to Dashboard when clicking on any tap
Do hard refresh `ctrl + shift + R` or `ctrl + f5`

# Image issues in templates
# Course Assign Notification Issue

# Credentials not working for LMS 

## User accounts Created but credentials emails not delivered 

When convert targets to drill user, user account Created but credentials emails not delivered.

# Phishing email arrive in Junk mail

# Need to delete the data for one or more target from campaign 

## Using `.live` & `.com` as Notification Senders for large or small numbers of employes

`.com` domains limited to a specific number of emails / per day,

While `.live` is not limited.

We can solve it through:

- `notifications@dphish.live` = Large Number of Employes (5000 for example)

- `notifications@dphish.com` = Small Number of Employes

## There are 2 stores:

1. Egypt Store
2. KSA Store

- Egypt Store = https://demoksa.dphish.live/ 
- KSA Store = https://store.dphish.live/

We can solve it through:

- **Egypt** Store = `Demoksa`

- **KSA** Store = `Store`

## notification@dphish.com

`.com` Notification Sender’s Credentials

We can solve it through:

- `TLS`: True
- `Password`: Vuxo957812
- `Port`: 587
- `Host`: smtp.office365.com
- `From`: Cybersecuiry Notification <notification@dphish.com>

## notification@dphish.live

`.live` Notification Sender’s Credentials

We can solve it through:

- `TLS`: True

- `Password`: BTLCyber1@!

- `Port`: 587

- `Host`: mail.dphish.live

- `From`: dPhish Notification <notifications@dphish.live>

## Difference between Support Mobile & Support Phone (in Settings > LMS)

We can solve it through:

- `Support Mobile` appears on the `footer of the LMS`.

- `Support Phone` appears on `Cyber_Awareness_Email`.

## Story editing error: translations: `[object Object]`

sometimes when you edit a story imported from store it shows this error

Another solution:

- First, try to delete the story, and then add it as a new story manually.

## `Risk Score` does not change, even after conducting a campaign

We can solve it through:

- There must be Drill Users on the platform.

## Adding the Client Notification Sender

The Notification Sender was not functioning properly and failed to send any emails

We can solve it through:

- First Know there is in exchange or o356 and write it in `setting`-> `platform`->`email service`

- then check the `Custom Notification Sender` is enable from `setting`-> `Notification Sender`

- if they on exchange then change `Sender Port` to 443

- if still not working make the `Sender From` email only

## Drill users don't receive otp 

when drill users login to platform, they didn't receive otp

We can solve it through:

- They should do a whitelist for notification sender.

Another solution:

- The customer can put his own notification sender.

## The fast login button in the email for the assign course isn't working and it's showing an error with the drill user.

We can solve it through:

- First, make sure the email was sent within a week; if it's been more than a week, it’s expired.

- If it's less than a week, press `Ctrl+Shift+R` to clear the cache on the client’s side.

Another solution:

- Send the drill user the link to their platform and tell them to forget the password.

## The email is flagged despite being whitelisted & trusted.

When Google blacklists a tracker, the email is flagged, even if it has been whitelisted.

We can solve it through:

- Changing the tracker with a new one will solve it.