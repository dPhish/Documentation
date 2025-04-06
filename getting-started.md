# Getting Started

## Home Dashboard
- Shows the `overall security status` of the company.
- Gives a `Risk Score` and shows if things are getting better or worse.
- Helps admins see what’s working and what needs fixing.

#### Main Parts:
##### 1. Risk Score
- Tells you how risky things are right now.
- Based on:
  - Phishing tests (60%)
  - Employee training (30%)
  - Leaked passwords (10%)

##### 2. Risk Score Chart
- A graph showing how the risk changes day by day.

---

## Do Dashboard
- Shows `phishing test results`.
- Tells you how employees react to fake phishing emails.

##### Key Sections:
1. **Campaign Stats**: How many emails were sent and how people reacted (clicked links, entered passwords, etc.).
2. **Top Campaigns**: Which tests worked best.
3. **Top Reporters**: Employees who reported phishing emails the most.
4. **Top Failures**: People or departments that failed the test the most.
5. **Email Reports**: How many phishing emails employees reported.

---

## Drill Dashboard
- Tracks `employee training progress`.
- Shows who finished the courses and who didn’t.

##### Key Sections:
1. **Courses Stats**: Total courses, users in training, missed deadlines.
2. **Awareness Progress**: How employees improve over time.
3. **Quiz Results**: Who passed or failed quizzes.
4. **Completed Courses**: How many finished everything.

---

## Detect Dashboard
- Shows `real threats` and `leaked data`.
- Helps spot problems fast.

##### Key Sections:
1. **Email Reports**: How many threats were reported.
2. **Leaked Credentials**: Which employees have leaked passwords.
3. **Threat Levels**: How dangerous reported emails are.
4. **Timeline**: When the threats were reported.

---

## DO : Do-Phish Module - Quick Summary
##### Purpose:
Test employees and email systems against phishing.

##### Two Main Functions:
1. **Phishing Simulation**: Sends fake emails to check if employees fall for phishing.
2. **Adversary Emulation**: Tests if email security blocks harmful emails.

##### Key Parts:
- **Campaigns**: Fake phishing tests.
- **Campaign Groups**: Run many campaigns at once.
- **Post Campaigns**: Train employees after they fail.
- **Emulations**: Test email security.
- **Attacks**: Simple phishing actions.

---

### Campaigns:
##### What is a Do-Phish Campaign?
- It's a `fake phishing attack` used to test how employees react.
- Helps `measure awareness` and `improve security`.

##### What You Can Do With Campaigns
1. Create phishing simulations (email, SMS, USB, QR codes).
2. Test employee actions (click links, open files, enter passwords).
3. Train employees after they fail (send courses, redirect to pages).

##### Campaign Management Basics
- Create Campaigns using an easy step-by-step wizard.
- View and Manage campaigns (edit, launch, clone, delete).
- Search and Filter campaigns by type, status, tags.
- Track Results: who opened emails, clicked links, or entered data.
- Post Actions: assign training or follow-ups to users who failed.

##### Campaign Target Management
- Add Targets manually, via CSV, or through LDAP.
- Track Target Actions: detailed info (IP, location, browser).
- Export Data: download reports on campaign results.
- Executive Reports: high-level summaries for management.

##### Types of Campaigns You Can Create
- Email with attachment
- Email with page
- Email/SMS with QR code
- USB attack
- HID device attack
- SMS phishing

### Campaign Groups - Quick Summary
##### What?
Group multiple campaigns together.

##### Why?
Manage them easily and get one combined `executive report`.

##### Key Actions:
1. View group
2. Edit group
3. Delete group
4. Download report for all campaigns

##### Inside the Group:
- See campaign names, types, status
- Remove or delete campaigns
- Track performance

---

### Post Campaigns - Quick Overview
##### What are they?
- Follow-up actions after a phishing test.
- Triggered when a user does something risky (like clicking a link or entering credentials).

##### Main Purpose
Teach users awareness after they fail a phishing test.

##### How It Works
- You set a **Condition** (e.g., Link Opened, Credentials Saved).
- If the condition happens, a **Reaction/Action** happens automatically.

##### Available Actions
- **Send Email**: Send an awareness email.
- **Assign Course**: Give the user a training course.
- **Redirect Page**: Send them to a page with tips or policies.
- **Add Tag**: Tag users for future campaigns.
- **Add to Drill Group**: Group them for bulk actions later.

##### Post Campaign Management
- You can **Create, View, Edit, and Delete** post campaigns.
- Search and Filter them easily.

---

### Emulation Campaigns - Quick Overview
##### What are they?
- Simulate `real email attacks` to test your `email security systems` (gateways, sandboxes).

##### Main Purpose
- Check if `email security` blocks dangerous emails properly.
- Make sure `filters` and `defenses` are working as they should.

##### How It Works
1. You create an `Emulation Campaign`.
2. Send fake `attack emails` at specific time intervals (to avoid auto-blocking).
3. Test is done on `one target`, because all emails go through the same security system.

##### Key Settings
- **Campaign Name & Description**
- **Interval (Seconds)**: Time between attacks
- **Sender**: Who sends the attacks
- **Target**: Who receives the test
- **Attacks**: Types of attacks/payloads sent

##### Actions You Can Do
1. View
2. Edit
3. Clone
4. Export
5. Delete
6. Open Ticket

---

### Attacks Tab - Quick Overview

##### What is it?
- A place to manage all `attacks` and `payloads` used in emulation campaigns.

##### Main Purpose
Organize, create, and manage `attack scenarios` and their `payloads`.

##### Key Features
- **List of Attacks**
  - Shows:
    - Name
    - Description
    - Type (URL, File)
    - Tactic & Technique
    - Author info
    - GUID (unique ID)

##### Actions You Can Do
1. View
2. Edit
3. Delete
4. Search & Filter (by Name, Type, Author, etc.)
5. Create New Attack
6. Add Payloads to an Attack

##### Payload Management
- **Payload** = The file or link used in the attack.
- You can:
  - Add New Payloads
  - `Edit` or `Delete` them
  - Upload payload files
  - Set status (Active/Inactive)
  - Track by MITRE ID

---

## Drill Module

##### What is it?
A training module to improve employee `security awareness`.

##### Key Features
- Create ``interactive`` courses with `quizzes`.
- Supports Arabic and `English`.
- Target specific user groups for focused training.
- Upload different content types:
  - PDFs
  - Videos
  - Infographics
- Organize content into course tracks for easy learning.

---

### 1. Courses

##### What are they?
- Interactive training courses to improve security awareness.

##### Main Features
- Courses have `quizzes`, `videos`, `PDFs`, and `infographics`.
- Support `Arabic` & `English` (multiple dialects).
- Courses are grouped by level (Beginner, Intermediate, Advanced).
- Each course has `deadlines`, `points`, and `progress tracking`.

##### What You Can Do
- Create courses with custom content.
- Assign `users`/`groups` manually or automatically.
- Add `quizzes` and `FAQs` to test knowledge.
- Track progress: who started, finished, or passed the quiz.
- Get feedback with comments and ratings.

##### Content Types
- Videos
- Presentations (PDF)
- Infographics
- Walkthroughs (PDF)

##### Course Management Actions
- View / Edit / Delete
- Search & Filter
- Assign by `Company`, `Group`, or `Post Campaigns`
- Track user actions with `Timeline Tracking`

---

### 2. Stories

##### What?
- Short, engaging `narratives` (videos or audio) to raise awareness.

##### Features:
  - No quizzes or progress tracking.
  - You can `create`, `edit`, `delete` stories.
  - Add `videos`, `descriptions`, and `durations`.

---

### 3. Tracks

##### What?
- A `group of courses` bundled into a single `learning path`.

##### Features:
  - Organize related courses.
  - Define Level, Scope, Intro.
  - Add `images`, reviews`, and `activate/deactivate` tracks.

---

### 4. Categories

##### What?
- Organize and `filter courses` into `categories` for better management.

##### Features:
  - Define `Name`, `Head`, and `Description`.
  - `Create`, `edit`, or `delete` categories.
  - Helps users find relevant courses easily.

---

### 5. Groups

##### What?
- Organize `users` into groups (e.g., by department or team).

##### Features:
  - Easy course assignment to `multiple users` at once.
  - Manage `Group Name`, `Description`, and `Users`.
  - `Create`, `edit`, or `delete` groups.

---

### 6. Announcements

##### What is it?
- `Awareness campaigns` sent by email to educate users.
- Focus on `security tips`, `company policies`, and `best practices`.

##### Main Features
- Works like phishing campaigns, but for `training`, not testing.
- Supports `scheduling`, `target selection`, and `templates`.
- No quizzes or tracking of mistakes—just `awareness`.

##### Campaign Setup
- Create Announcement
- Choose Category (Awareness, Policy, Others)
- Add `Template` & `Page`
- Select `Targets` (users/groups)

##### What You Can Do
- View / Edit / Delete announcements
- Track Engagement:
  - Emails sent, opened, accepted
- Monitor Targets (track actions, IP, browser info)

---

### 7. Users

- Manage all `LMS users`.
- Actions:
  - Create / Edit / Delete users
  - Change passwords
  - Notify inactive users
- Track `user status` (Active/Inactive) and `creation date`.

---

### 8. Badges

- Reward users when they achieve certain points.
- Actions:
  - Create / Edit / Delete badges
- Define:
  - Name
  - Description
  - Condition (when they get the badge)

---

### 9. Policies

- Upload and manage `company policies`.
- Users can `view` and `accept` policies in the LMS.
- Actions:
  - Create / Edit / Delete policies
  - Track who viewed or accepted them.

---

### 10. Content Logs

- Track `user interactions` with course content.
- Shows:
  - Which user viewed what content
  - When it was viewed
- Actions:
  - Filter logs by user or course
  - Export logs (CSV, XLS, JSON)

---

## Detect

##### What is it?
- A platform that `detects and analyzes phishing emails`.
- Gives security teams `one dashboard` to review reports and take action.
- Includes `ticketing`, `triage`, and `response tools`.

##### Main Components:

###### 1. Analyzed Emails
- Shows all reported phishing emails in one place.
- Key details include:
  - Email Subject
  - Source (Add-on, API, Web)
  - Severity (Low to Critical)
  - Links, Attachments
- Actions available:
  - View / Rescan / Open Ticket
  - Change Status (Open, In Progress, Resolved)
  - Response: Delete, Quarantine, Search by Sender/Subject

###### 2. Leaked Credentials
- Tracks `employee credentials` exposed in:
  - Malware logs
  - Public data breaches
- Actions:
  - Enrich (detailed leak info)
  - Open Ticket for investigation
  - Rescan leaked data
- Impacts Risk Score (up to 10% of total risk).

###### 3. Indicators of Compromise (IOCs)
- Lists `threat indicators` extracted from phishing reports.
- Includes:
  - IP addresses
  - URLs
  - File hashes (SHA256)
- You can `filter` or `export` this data for reports.

###### 4. Response Actions
- Search for similar emails in the entire organization.
- **Take actions like**:
  - Delete or Quarantine emails
  - Search by Sender or Subject
  - Mass actions on multiple emails.

---

### Analytics

##### What is it?
- A `dashboard` to track and analyze all activities on the platform.
- Covers `Campaigns (Do)`, `Training (Drill)`, and `Threat Detection (Detect)`.
- Helps admins `monitor performance` and `export reports`.

##### Main Sections:

###### 1. Reports
- Shows `detailed reports` for Do, Drill, and Detect activities.
- Includes `Executive Reports` that summarize everything in one file.
- Reports are downloadable in `CSV`, `XLS`, or `JSON` formats.

###### 2. Trackers
- Displays `all user actions` during phishing simulations:
  - Emails opened
  - Links clicked
  - Credentials submitted
- Shows details like:
  - Campaign name
  - Target user info
  - Device info
  - Public IP
- You can `search`, `filter`, and `export` the data.

###### 3. Credentials
- Lists credentials entered by users during `phishing simulations`.
- Displays:
  - Campaign name
  - Target name & email
  - Department
  - Submission date
- `Passwords are never stored`, only credentials logs.
- You can `search`, `filter`, and `export` the data.

---

## Utilities Module

The Utilities module helps manage campaign components like `Targets`, `Pages`, `Templates`, and `Senders`. It ensures campaigns (Phishing & Announcements) are organized and efficiently executed.

### Targets
- **Purpose**: Manage people or devices used in campaigns (Phishing & Emulation).
- **How to Add Targets**:
  1. Manual Entry.
  2. CSV File Upload.
  3. LDAP Integration.
  4. Azure/Office 365 Integration.
- **Target Details include**: Name, Email, Phone, Department, etc.
- **Actions**: View, Edit, Delete, Create LMS Drill Accounts.
- **Export/Import Options**: Export target lists, import via CSV/LDAP/Azure.

### Pages
- **Purpose**: Custom pages for phishing (collect credentials) or announcements (awareness).
- **Features**: Create, Edit, Clone, Delete pages.
- **Languages**: English, Arabic, German, French.
- **Tools**: Built-in text editor and IDE for page design.

### Templates
- **Purpose**: Email templates for phishing or awareness campaigns.
- **Features**: Create, Edit, Clone, Delete templates.
- **Details**: Name, Subject, Language, Tags.
- **Tools**: Same IDE as Pages for designing emails.

### Senders
- **Purpose**: Manage email senders used in campaigns.
- **Details**: Name, Username, Host, Port, From email, Category (Phishing or Announcement).
- **Features**: Add, Edit, Clone, Delete senders.
- **Export Data**: Download reports of all senders.

### Drill Accounts (LMS Access)
- **Purpose**: Provide LMS (Learning Platform) access to targets for awareness training.
- **Methods**:
  1. Create accounts for all targets.
  2. Create account for one target.
  3. Auto-create accounts when targets are added.
- **Users get credentials by email when accounts are created.

---

## Platform Module

The Platform module simplifies the management of key assets across `admin roles`, `tickets`, `file management`, `logs`, `email services`, and more. It provides control over user access, system operations, and ensures secure communication.

### Roles and Permissions
- **Purpose**: Define and control user access.
- **Key Features**:
  - Create roles and assign permissions.
  - Group permissions for better management.
  - Bulk assignment of permissions.
  - Control what each user can access/do.
- **Future Enhancements**:
  - Role-based dashboards.
  - Import/export of permission settings.

### Users Management
- **Purpose**: Manage platform admins.
- **Key Features**:
  - Add/Edit/Delete admin users.
  - Control user privileges and activation status.
  - Notify users on creation (optional).
- **Actions**:
  - Change password.
  - Assign roles.

### Ticketing System
- **Purpose**: Manage service requests/issues.
- **Key Features**:
  - Open/view/close tickets.
  - Assign tickets to users.
  - Notify users upon assignment.
- **Modules Supported**: Campaigns, Emulations, Analyzed Emails, Leaked Credentials.

### File Management
- **Purpose**: Host and organize files (images, videos, etc.) for campaigns.
- **Key Features**:
  - Upload/download assets.
  - Secure storage and usage in campaigns.

### Logs
- **Purpose**: Track admin activities on the platform.
- **Key Features**:
  - View logs with timestamps, IPs, actions.
  - Filter by method/user.
  - Audit and monitor platform usage.

### Tasks
- **Purpose**: Monitor all running tasks (campaigns, emulations).
- **Key Features**:
  - Terminate tasks from the tasks panel.
  - Track task history and status.

### Store
- **Purpose**: Sync the latest assets (Pages, Templates, Senders, Courses, Attacks).
- **Key Features**:
  - Sync all or selective assets.
  - Import from the store without impacting existing data.

### Email Services
- **Purpose**: Integrate and manage email services (Google, Office365, Exchange, LDAP).
- **Key Features**:
  - Setup secure email communication.
  - Enable TLS, SSO, and Response services.
  - Sync user accounts from Active Directory.

### Email Templates
- **Purpose**: Manage built-in email templates for notifications.
- **Key Features**:
  - Edit email content (limited to provided templates).
  - 18 templates available (EN & AR).
  - Use for OTP, notifications, course assignments, etc.