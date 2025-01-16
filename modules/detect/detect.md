## Overview

> dPhish Detect centralizes the detection and analysis of phishing emails. It aggregates all reported emails from various sources into a unified dashboard, enabling security teams to investigate and take appropriate triaging actions. Security analysts can examine these emails in great detail, as each reported email is an exact replica of what the user received, including all attachments and URLs for further investigation. Each reported email is assigned a unique identifier, allowing the security team to track them easily.  dPhish Detect includes an integrated built-in ticketing system to streamline the process of analyzing and triaging reported emails. 
Additionally, the module allows exporting various statistics about the reported emails, such as their severity, detection status, source, and the reporter’s email address.


## Main Components

- Description automatically generated The dPhish Detect module consists of 3 sub-modules each performing a specific task:  

    - `Analyzed Emails`: The main module in dPhish Detect is responsible for displaying reported emails in a unified dashboard, enabling security teams to investigate them. 

    - `Leaked Credentials`: Tracks the credentials of employees registered on the platform for any leaks on the Dark Web. 

    - `IOC`: A dashboard that aggregates and displays Indicators of Compromise (IoCs) extracted from reported emails, along with the available threat intelligence for these IoCs. 