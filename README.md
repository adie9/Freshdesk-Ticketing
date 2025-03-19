# Freshdesk-Ticketing
For this project, I created a ticketing system using Freshdesk. I wanted to familiarize myself with the ticketing system and process used in most helpdesk jobs, and I figured this would be a good way to do so.

## Overview

### Portal Setup
I created a free Freshdesk account using my email and a company name: "AG Company". After creating the account, I was greeted with the ticketing page:

![Ticket_Dashboard](/images/Ticket_Dashboard.png)

### Email Server
I created a new email account to handle the incoming requests from the ticketing system. I navigated to Admin > Email and clicked "New support email": 

![Support Email](/images/Support_Email.png)

To test if the email was configured correctly, I sent a test email to see if the request would show up in the ticketing system. 

![Test_Email](/images/Test_Email.png)

![Test_Email_Success](/images/Test_Email_Success.png)

### Ticket Automation
Next, I wanted to try and route tickets based on the content found in the request. For example, if a request contained "password reset", the ticket should be automatically routed to the group "Level 1 IT Support". To do this, I first needed to create the group. I navigated to Admin > Groups and created the group:

![Group_Creation](/images/Group_Creation.png)

Now that the group was created I needed to create a rule. I navigated to Admin > Automation and clicked on "New Rule". A rule has three components: 1) **Event** (Which just indicates the rule runs upon ticket creation), **Condition** (Sets the conditions for the rule to match), and **Action** (What the rule will do when conditions are met). For the "Send Password Resets to Level 1 IT Support" rule, I set the Condition to "Subject" or "Description" containing "password reset", and the Action to "Assign to Group 'Level 1 IT Support'".

![Password_Reset_Rule](/images/Password_Reset_Rule.png)

I submitted a ticket via the "Submit a Ticket" page in the company portal, with "password reset" in the Subject and Description, and checked the Group that the ticket was assigned to once it popped up in the ticketing system:

![Submit_A_Ticket](/images/Submit_A_Ticket.png)

![Group_Rule_Success](/images/Group_Rule_Success.png)

### Closing Tickets
To simulate the role of an agent, I'd take ownership of the ticket by assigning myself to the ticket and change the status to "Pending". Once the issue is resolved, I send an reply email to the user and change the ticket status to "Resolved".

![Resolved_Ticket](/images/Resolved_Ticket.png)

## What I Learned
After completing this project, I was able to familiarize myself with a ticketing system and its processes such as configuring a support email, automating ticket routes, and responding to/closing tickets. I was very keen on the idea of ticket automation, as agents were able to receive tickets based on what group they were in. No one from the group "Billing" would receive tickets addressed to the group "Level 1 IT Support". The automation system provided an overall organized experience.
