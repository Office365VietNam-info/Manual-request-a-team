# Manual-request-a-team
Use PowerAutomate to make a flow for request approval a team in Microsoft Teams.

# Architecture - Manual request a team
This's basic Architecture for this flow:
A. User should submit their requests via MS Forms.
B. PowerAutomate will store request information in SharePoint list.
C. Send approval requesting to a channel in a team for getting approval from admins.
D. PowerAutomate check condition to decide create a team.
E. After create a team, it will update information into SharePoint list and then send notification to requested user.
![alt text](https://github.com/Office365VietNam-info/Manual-request-a-team/blob/main/Architecture/Architecture%20-%20Manual%20request%20a%20team.png?raw=true)

# Preparation
A. A Microsoft Forms for front end. Forms have 3 basic questions:
1. Name of team want to create
2. Business purpose or description
3. Type of team is Private or Public
![alt text](https://github.com/Office365VietNam-info/Manual-request-a-team/blob/main/Architecture/Forms.png?raw=true)

B. A SharePoint site with a customize list for storing requests. Columns should include:
1. ID: number of submited form/form id.
2. Name of team want to create
3. Business purpose or description
4. Type of team is Private or Public
5. Status: Approved or rejected
6. Comment is Approval comment
![alt text](https://github.com/Office365VietNam-info/Manual-request-a-team/blob/main/Architecture/SP%20List.png?raw=true)

C. A PowerAutomate for business logics. Get the template at here: https://bit.ly/tlrequestateam
This PowerAutomate template was included all business logics need for running this flow.

# Implement step by step
1. Prepare as the Preparation stage
2. Import PowerAutomate template and config connectors and parameter.
3. Enjoy

# Demo
[![Watch the video](https://img.youtube.com/vi/V49l9U56bWM/hqdefault.jpg)](https://youtu.be/V49l9U56bWM)
