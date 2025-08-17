# Main Page

**Response**
Once an investigation of a reported email is complete and the final verdict is malicious, it’s crucial to accurately assess the situation to respond to the threat. The response feature allows analysts to search for an email, using either the sender or the subject of the email, over every mailbox in the organization. This search process, also called Scope, will aggregate all emails in the organization that match the search criteria and display them in a listing to the analyst. The UI of the response page is simple yet powerful:

## Response Details:
1. **Delete**: Delete the selected email from the view page. This will delete the email from the mailbox of the reported.
2. **Quarantine**: Same as delete, except the mail will be quarantined instead of deleted.
3. **Scope by Sender**: Searches for emails in the organization that originated from sender as in the reported email.

![Detect-Phish response main!](../../assets/detect/response/main.png "Detect-Phish response main")

4. **Scope by Subject**: Searches for emails in the organization that have the same subject as the reported email.
5. **Search**: Once the search is over, the page is populated with emails that matched the search criteria. Analysts can then take actions on these emails such as mass deletion or mass quarantine.
6. **Delete**: Deletes the selected email from the dashboard listing. Any tickets opened on the deleted entry will be deleted as well. Note that this DOES NOT delete the email from the reporter’s mailbox, that what response does, it just deletes it from the platform.

### Download Sample Template  
- This button allows you to download a sample CSV template that you can fill in with your data.  
- The template contains three columns:  
    1. **Email** – the recipient’s email address.  
    2. **Subject** – the subject line of the email.  
    3. **Sender** – the email address of the sender.  

### Upload File  
- A file upload box labeled “Upload file here”.  
- When clicked, it opens a file selector so you can choose the CSV file you’ve filled with your data.  
- Once uploaded, the platform will be ready to take action on the listed emails.  

### Choose Action  
- After uploading the file, you can select the action to perform on each email in the list.  
- Available actions include:  
    1. **Quarantine Email** – isolate the email to prevent access.  
    2. **Delete Email** – remove the email from all mailboxes.  

### Execute Action (Respond)  
- After selecting the desired action, you click the Respond button.  
- This triggers the system to perform the selected action on all mailboxes containing the listed emails.