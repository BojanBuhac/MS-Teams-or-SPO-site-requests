# MS Teams or SPO site requests solution
As part of the SPO governance many organizations are disabling creation of MS Teams and SPO sites for end users. This solution is for those organizations, as it allows them to deploy this application that users can use to submit requests for new MS Teams or SharePoint Online sites. As part of the governance solution includes 2 step approvals (requester manager and IT).
### App main view
![screenshot](/images/main.png)
### New site types
![screenshot](/images/new.png)
### New site additional owners, type and quota
![screenshot](/images/quota.png)
### App config
![screenshot](/images/config.png)
# Solution architecture
## Database
This solution stores data in 3 SharePoint Online lists:

![screenshot](/images/spolists.png)
- Teams Request Settings - app solution settings that are controlable thru app
- Teams Request - list of requests submited by end users
- Teams Request Approver - list of approvers for each category (department or country or city or ...)
## Application
Solution is provided as Power App Solution

![screenshot](/images/solution.png)
- Canvas app
- Power Automate flows
  - Main approval flow
  - Get SPO url for teams site flow
- Connection references
- Environment variables
# Deployment
1. Download all CSV files from Solution folder
2. Create new SharePoint site where app data will be hosted
3. ...
