# SC-300T00 Microsoft Identity and Access Administrator - All Modules Errata

# NOTE:  At the end of each module of labs, delete all the resources created in the module

# Implement an identity management solution (~190 Minutes)

## Lab 0 - Create a Microsoft Azure Pass Subscription (10 Minutes)
Step 2:  Activate your subscription
Leave Name and email as is, enter your information in the remaining fields – must include a valid phone number

Read this at the very end of Lab 0: 

# Important note: a later lab requires a time-consuming deployment. To save your time later, we suggest that you kick off that portion of the lab now so it’s ready when you get there. To do that:

After completing Lab 0 use the next button to skip to Lab 07
Complete Lab 07 Exercise 1 Task 1 
Once the deployment has started use the previous button to return to Lab 01
Continue with Lab 01, and Lab 07 should be ready when you get there

## Lab 01 – Manage user roles (30 Minutes)

Exercise 1 – Create a new user and test their application admin rights
Task 1:  Add a new user
Step 6:  Use the following password
	Pass@word!
Task 2: Bulk addition of users using PowerShell
Step 2: After running Install-Module AzureAD run Import-Module AzureAD to import the module prior to use
Exercise 4 - Bulk import of users
Task 1 - Bulk operations for creating users with a .csv file
Step 6:  After opening the .csv file paste your tenant name from the resources tab in the lab guide at the bottom of the file
Use the replace feature in Notepad to replace <<<enter your domain name>>>
After pasting delete your tenant name you pasted at the bottom of the file 
Task 2:  Bulk addition of users using PowerShell
Step 7:  Copy and paste your tenant name from the Azure Portal notepad
Paste the New-Aduser cmdlet into notepad
Replace the labtenname.com with your tenant name
Copy and paste cmdlet into PowerShell
Exercise 6 - Add a Windows 10 license to a user account
Task 1 - Find your unlicensed user in Azure Active Directory
Step 5:  Click edit properties > Settings tab to verify Usage location
Lab 02 – Working with tenant properties (15 Minutes)
Exercise 3 - Setting your privacy information
Task 1 - Adding your privacy info on Azure AD, including Global privacy contact and Privacy statement URL
Step 2:  Will not paste.  In the lab environment use edge to browse to the github.com repository to the pdf and copy URL from browser
Use the following steps to get to the PDF
https://github.com 
On the github page search for SC-300
Select MicrosoftLearning > Allfiles > Labs > Lab2 > SC-300-Lab_ContosotPrivacySample.pdf
Copy URL
Lab 03:  Assigning licenses using group membership (25 Minutes)
Exercise 1 - Create a security group and add a user
Task 4 - Confirm the SteOffice 365 license
Step 4:  it may take up to 5 minutes for the license to be applied, logout wait a few minutes log back in
Lab 04:  Configure external collaboration settings (5 Minutes)
No errata
Lab 05 -Add guest users to the directory (5 Minutes)
Exercise 1 – Add guest user to the directory
Step 4:  Use the New user drop down box, select Invite external user
Exercise 2 - Invite guest users in bulk
Task 1 - Bulk user invite
Use the step as an example, do not actually submit the file
Task 2 - Invite guest users with PowerShell
PowerShell was installed in a previous lab you may be able to start at step 4
Lab 06 – Add a federated identity provider (25 Minutes)
Exercise 1 – Configure identity providers
Task 1- Configure Google to be used as an identity provider
Note:  Create a Gmail account for use in this lab, I recommend something like this
	Initialssc300@gmail.com (FFsc300@gmail.com)
	If the account is taken use a recommended one – Note your username and password
Step 1:  Does not paste – type in manually
Step 5:  In the Application type menu, select Web application. Give the application a suitable name, like Azure AD B2B. Under Authorized redirect URIs, add the following URIs:
Copy and paste the URLs into notepad, paste 1 line at a time do not include the –
Copy the client ID and Secret and paste in notepad
Lab 07 – Add Hybrid Identity with Azure AD Connect (75 Minutes)
Exercise 1 – Setup On-Premises infrastructure
Task 1 – Create the on-premises Active Directory infrastructure
Step 1:  The link may not paste in the lab environment, if not enter the following in Edge
	https://github.com/maxskunkworks/TLG/tree/master/tlg-base-config_3-vm
Step3:  when deplying the VM choose size  Standard_D2s_v2
Note the DNS label prefix you use – I used retSC300
Note:  If you jumped here after completing Lab 0, do not wait for the deployment to finish, press Previous to return to Lab 1
Task 2 - Configure the lab environment Azure VMs
Step 1:  Password is incorrect use   demo@pass123
Steps 2, 3, 4, 5 it easier to run each one in a separate tab in the PowerShell ISE
There is no Task 4
Task 5 - Configure contoso.local Active Directory
Step 1:  Password is incorrect use   demo@pass123
After connecting, launch IE download and install Chrome.  Then complete task 5 in Chrome
Replace Step 2 with the following:  
Browse to https://github.com/microsoft/MCW-Hybrid-identity
Select the Code box and click on Download zip.
Browse to the downloaded file and extract
Browse to c:downloads\MCW-hybrid-identity-main\ MCW-hybrid-identity-main\Hands-on labs\studentfiles
Skip to Step 5
Step 8:  After running the script open Active Directory Users and Computers to verify the Demo Accounts OU has been created and populated with users and groups.
	Note:  when the script is running you may see red flashing by, ignore
	Do not run the script a second time, it will delete the Demo Accounts OU
Step 9:  Paste into another tab in the ISE before running
Step 10:  Paste into another tab in the ISE before running
Exercise 2: Integrate an Active Directory forest with an Azure Active Directory tenant
Task 1: Create an Azure Active Directory tenant and activate an EMS E5 trial
Step 6:  recommend initials then Contoso when creating the initial domain name
	Note:  do not close the Captia once it says Tenant Creation in Progress
Step 7:  Select navigate to tenant when successful
Skip to Step 11
Task 3: Purchase a custom domain name
Step 1:  Navigate to Azure Active Directory > Manage tenants > Select the Contoso Marketing Tenant > Switch 
Skip Step 2
Step 9:  change the email to a valid email you use
Step 12:  If deployment fails continue with the next task.
Your custom domain name will not verify but the lab will still work
Task 6: Install Azure AD Connect
Step 18:  Password is demo@pass123
Step 25:  Password is demo@pass123
Task 9: Initiate and verify directory synchronization
Step 11:  In Chrome
Task 11: Perform Hybrid Azure AD join
Step 3;  Login as  corp\AGAyers
NOTE:  At the end of module, delete all the resources created in the module
 

Implement an authentication and access management solution (~150 Miuntes)
Lab 08 – enable Azure AD multifactor authentication (15 Minutes)
IMPORTANT - An Azure AD Premium license is required for this exercise.
	O365 AAD has already been provisioned 
Exercise 1 - Review and enable Multi-factor Authentication in Azure
No Errata
Lab 09 – Configure and deploy self-service password reset (15 Minutes)
Exercise 1 - Create a group with SSPR enabled and add users to it
Task 3 - Register for SSPR with Alex
Step 4:  Click on Security info > + Add sign-in method 
Lab 10 – Azure AD Authentication for Windows and Linux Virtual Machines (30 Minutes)
Exercise 1 - Login to Windows Virtual Machines in Azure with Azure AD
Task 1 - Create a Windows Virtual Machine with Azure AD login enabled
Use the following setting on the Basic tab
Resource group;  myDemoRG
Virtual machine name:  myVM1
Availability options:  No infrastructure redundancy required
Image:  Windows Server 2019 Datacenter – Gen 1
Username:  demouser
Password:  demo@pass123
Task 2 - Azure AD login for existing Azure Virtual Machines
Step 4:  Choose your Global Admin as a member
Exercise 2 - Login to Linux Virtual Machines in Azure with Azure AD
Task 1 - Create a Linux VM with system assigned managed identity
Use the following setting on the Basic tab
Resource group;  myDemoRG
Virtual machine name:  myVM2
Availability options:  No infrastructure redundancy required
Authentication type:  Password
Username:  demouser
Password:  demo@pass123
Task 2 - Azure AD login for existing Azure Virtual Machines
Step 4:  Choose your Global Admin as a member
Lab 11 - Assign Azure resource roles in Privileged Identity Management (10 Minutes)
No errata
Lab 12 – Manage Azure AD smart lockout values (5 Minutes)
No Errata
Lab 13 – Implement and test a conditional access policy (30 Minutes)
No Errata
Lab 14 – Enable sign in and user risk policies (10 Minutes)
No Errata 
Lab 15 – Configure an Azure AD multi-factor authentication registration policy (10 Minutes)
No Errata
Lab 16 – Using Azure Key Vault for Managed Identities (20 Minutes)
Exercise 1 - Use Azure Key Vault to manage Virtual Machine identities
Task 1 - Create a Windows Virtual Machine
Task 2 - Create a Key Vault
Step 6:  May need to add your initials to the Key vault name
Task 5 - Access data with Key Vault secret with PowerShell
Step 2: returns unable to resolve the name.  Open a PowerShell Prompt.  Use IP config to determine the computer’s IP address.  Replace the address in the CMDLET with the IP address
NOTE:  At the end of module, remove all policies.  Delete all the resources created in the module

 
Implementing access management for apps (~90 Minutes)
Lab 17 – Defender for Cloud Apps application discovery and enforcing restrictions (10 Minutes)
Exercise 1 - Defender for Cloud Apps discovery
Task 1 - Discovery apps in Defender for Cloud Apps
Step 1:  Link does not paste correctly in the lab environment, open a new tab in edge.  Type https://security.microsoft.com
Lab 18 – Defender for Cloud Apps Access and Session Policies (20 Minutes)
Skip does not work as written 
Lab 19 – Register an application (30 Minutes)
Exercise 1 - Register an application
Task 2 - Configure platform settings
You will not make any changes, you are only exploring the options
Step 6:  Hit the x to close the platform configuration window
Task 5 - Add a scope
Step 7:  Populate the fields with the example content
Lab 20 – Implement access management for apps (5 Minutes)
No Errata
Lab 21 – Grant tenant-wide admin consent to an application (15 Minutes)
Exercise 1 - Admin Consent
Task 1 - Grant admin consent in App registrations (Skip task, option has been removed
NOTE:  At the end of module, remove any policies or security settings.  Delete all the resources created in the module
 
Plan and implement an identity governance strategy (~130 Minutes)
Lab 22 – Create and manage a catalog of resources in Azure AD entitlement management (15 Minutes)
No Errata
Lab 23 – Add terms of use and acceptance reporting (20 Minutes)
Exercise 1 - Set up a Term of Use and test them
Task 1 - Add terms of use
Step 9:  Browse to the following location, and download the file
https://github.com/MicrosoftLearning/SC-300-Identity-and-Access-Administrator/blob/master/Allfiles/Labs/Lab26/Contoso_TermsOfUse.pdf
Lab 24 – Manage the lifecycle of external users in Azure AD identity Governance settings (5 Minutes)
No Errata
Lab 25 – Create Access Reviews for Internal and External Users (5 Minutes)
No Errata
Lab is an explore lab, 
Lab 26 – Configure Privileged Identity management for Azure AZ Roles (30 Minutes)
Exercise 2 - PIM with Azure AD roles
Step 6:  URL will not paste, open a new tab in Edge and type the URL in.
Lab 27 – Microsoft Sentinel Kusto Queries for Azure data sources (30 Minutes)

Exercise 1 - Configure Microsoft Sentinel for Kusto Queries
Task 3 - Run Kusto query on User activity
Step 3:  Search for User IDs
Step 7:  Search for Anomalous sign-in location by user account and authenticating application
Lab 28 – Monitor and manage security posture with Identity Secure Score (15 Minutes)
Exercise 1 - Using Identity Secure Score to monitor and manage identity security posture
Task 2 - Execute an improvement action
Step 1:  Select Protect all users with a user risk policy
NOTE:  At the end of the module, remove any policies or security settings.  Delete all the resources created in the module
