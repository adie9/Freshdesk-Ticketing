# Freshdesk-Ticketing
For this project, I created a ticketing system using Freshdesk. I wanted to familiarize myself with the ticketing system and process used in most helpdesk jobs, and I figured this would be a good way to do so.

## Overview

### Portal Setup
I created a free Freshdesk account using my email and a company name: "AG Company". After creating the account, I was greeted with the ticketing page:

![Ticket_Dashboard](/images/Ticket_Dashboard.png)

### Email Server
I created a new email account to handle the incoming requests from the ticketing system: 

![Support Email](/images/Support_Email.png)

To test if the email was configured correctly, I sent a test email to see if the request would show up in the ticketing system. 

![Test_Email](/images/Test_Email.png)

![Test_Email_Success](/images/Test_Email_Success.png)

### Ticket Automation
Next, I wanted to try and route tickets based on the content found in the request. For example, if a request contained "password reset", the ticket should be automatically routed to the group "Level 1 IT Support". To do this, I first needed to create the group. I navigated to Admin > Groups and created the group:

![Group_Creation]

Now that the group was created I needed to create a rule. I navigated to Admin > Automation and clicked on "New Rule". A rule has three components: 1) **Event** (Which just indicates the rule runs upon ticket creation), **Condition** (Sets the conditions for the rule to match), and **Action** (What the rule will do when conditions are met).

## What I Learned
After completing this project, I was able to familiarize myself with a ticketing system and its processes such as configuring a support emai, automating ticket routes, and responding to/closing tickets.
