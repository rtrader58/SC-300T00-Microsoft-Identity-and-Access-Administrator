# SC-300T00 Microsoft Identity and Access Administrator - All Learning Paths Errata

# NOTE:  ENSURE YOU SELECT SAVE WHEN YOU FINISH THE SELECTED LABS 1-9, 12-15, 17-26 and 28

# Learning Path 2: Implement an identity management solution (~120 Minutes)

# Optional - Lab 07 - Cannot be accomplished in the current environment - requires creating a trial subscription

## Lab 01 – Manage user roles (30 Minutes)

### Exercise 1 – Create a new user and test their application admin rights

Task 1:  Add a new user<br>
Step 1:  Credentials are located in the Resources drop down - requires MFA with use of an Authenticaton App on phone<br>
Step 5:  Open Notepad and paste the the user name and auto generated password<br>

Task 2 - Login and try to create an app<br>
Step 3:  Use the user password provided in the Resources drop down - requires MFA with use of an Authenticaton App on phone<br>

### Exercise 4 - Bulk import of users

Task 1 - Bulk operations for creating users with a .csv file<br>
Step 6:  After opening the .csv file paste your tenant name from the resources tab in the lab guide at the bottom of the file<br>
Use the replace feature in Notepad to replace <<<enter your domain name>>><br>
After pasting delete your tenant name you pasted at the bottom of the file <br>

Task 2:  Bulk addition of users using PowerShell<br>

Task 2: Bulk addition of users using PowerShell<br>
Step 1: To determine PowerShell version type $PSVersionTable and press “Enter.”
If upgrade needed - Open the browser type https://aka.ms/PSWindows - Under Installing PowerShell 7 - click on MSI package - Click on PowerShell-7.5.0-win-x64.msi - Click open file - Follow the prompts to install <br>
Close PowerShell <br>
Search for and Open PowerShell 7 <br>

Step 6:  Open Notepad<br>
Paste $PwProfile command into Notepad <br>
Replace <Enter a complex password you will> with User password from the Resources drop down<br>
copy and paste from Notepad into the PowerShell prompt <br>

Step 7: Open Notepad  <br>
Paste the command in Notepad <br>
Replace <labtenantname.com> with your tenant <br>
Copy and paste from Notepad into the PowerShell prompt <br>

### Exercise 6 - Add a Windows 10 license to a user account

Task 1 - Find your unlicensed user in Azure Active Directory<br>
Step 5:  Click edit properties > Settings tab to verify Usage location<br>

Task 2 - Add a Windows license to Raul  <br>
Step 6:  + Assign licenses <br>

## Lab 02 – Working with tenant properties (15 Minutes)

### Exercise 3 - Setting your privacy information

Task 2 - Check your Privacy Statement  <br>
Step 1: Type https://portal.azure.com  <br>

## Lab 03:  Assigning licenses using group membership (25 Minutes)

Exercise 1 - Create a security group and add a user<br>
Task 1 - Check to see if Delia Dennis has access to Office 365<br>
DeliaD password is the User Password not the Admin password<br>

Task 3 - Add an Office license to sg-SC300-O365<br>
Step 9: Should read sf-SC300-0365 not Raul<br>

Task 4 - Confirm the Office 365 license<br>
Step 4:  It may take up to 5 minutes for the license to be applied, logout wait a few minutes log back in<br>

## Lab 04:  Configure external collaboration settings (5 Minutes)

### No errata

## Lab 05 -Add guest users to the directory (5 Minutes)

### Exercise 1 – Add guest user to the directory

Step 4:  Use the New user drop down box, select Invite external user<br>

### Exercise 2 - Invite guest users in bulk<br>

Task 1 - Bulk user invite<br>
Use the step as an example, do not actually submit the file<br>

Task 2 - Invite guest users with PowerShell<br>
PowerShell was installed in a previous lab you may be able to start at step 4<br>

## Lab 06 – Add a federated identity provider (25 Minutes)

### Exercise 1 – Configure identity providers

Note:  Create a Gmail account for use in this lab, I recommend something like this<br>
Initialssc300@gmail.com (FFsc300@gmail.com)<br>
If the account is taken use a recommended one – Note your username and password<br>

Task 1- Configure Google to be used as an identity provider<br>

### Create a new project:

Step 5: Includes steps 6 and 7: Click Get started > Create an App Name > Select Next > Select External > add your gmail > Click Next > Select I agrree > Click Continue > Click Create<br>
Step 8: Click Branding > Click + Add domain > follow steps 9 -11 > click Save<br>
Step 11: Click Overview > Click Create OAth Client <br>
Step 13:Click +Add URI Copy and paste the URLs into notepad, paste 1 line at a time do not include the – <br>
Step 14: Copy the client ID and Secret and paste in notepad<br>

Task 2 - Add a test user<br>
Step 2: Select Audience > Select + Test User<br>

### Exercise 2 - Configure Azure to work with an External identity provider

Task 1 - Configure Microsoft Entra ID for Google federation<br>
Step 5 and 6: Select Configure next to Google<br>

Task 3 - Accept the invitation and login<br>
Step 3: If you get an error > close the tab and select accept invite again<br>
Step 4: Select send code<br>

Task 4 - Login to Microsoft 365 using your Google account<br>
Step 7: Enter the code sent to your email<br>

## SKIP - Lab 07 – Add Hybrid Identity with Microsoft Entra Connect (75 Minutes)

### Exercise 1 – Setup On-Premises infrastructure

Task 1 – Create the on-premises Active Directory infrastructure<br>
Step 1:  Open and additional tab in the edge browser to paste.  The link may not paste in the lab environment, if not enter the following in Edge<br>
https://github.com/maxskunkworks/TLG/tree/master/tlg-base-config_3-vm<br>
Step 3:  Set password to: I used the user password under Resources<br>
When deplying the VM choose size  Standard_DS2_v2<br>
DNS label prefix you use – I used retSC300<br>

### Note:  If you jumped here after completing Lab 0, do not wait for the deployment to finish, press Previous to return to Lab 1<br>

Task 2 - Configure the lab environment Azure VMs<br>
Step 1:  Password is incorrect use you set<br>
Steps 2, 3, 4, 5 it easier to run each one in a separate tab in the PowerShell ISE<br>

There is no Task 4<br>

Task 5 - Configure contoso.local Active Directory<br>
Step 1:  Password is incorrect use you set<br>
After connecting, launch IE download and install Chrome.  Then complete task 5 in Chrome<br>
Replace Step 2 - 4 with the following: <br> 
Browse to https://github.com/microsoft/MCW-Hybrid-identity/tree/main/Archive/Hands-on%20lab/studentfiles<br>
Click on CreateDemoUsers.csv > On the Code box > click on Download Raw file > click back button on browser<br>
Click on CreateDemoUsers.ps1 > On the Code box > click on Download Raw file<br>
Step 8:  After running the script open Active Directory Users and Computers to verify the Demo Accounts OU has been created and populated with users and groups.<br>
Note:  when the script is running you may see red flashing by, ignore<br>
Do not run the script a second time, it will delete the Demo Accounts OU<br>
Step 9:  Paste into another tab in the ISE before running<br>
Step 10:  Paste into another tab in the ISE before running<br>

### Exercise 2: Integrate an Active Directory forest with an Azure Active Directory tenant

Skip Task 1: Create an Azure Active Directory tenant and activate an EMS E5 trial<br>

There is no Task 3 and 4

Task 5:  Configure DNS suffix in the Contoso Active Directory forest <br>
Step 5:  Password is incorrect use you set<br>
Step 6:  Use Contoso.com as alternate name
Step 7:  In line 1 of the script replace <custom_domain_name> with Contoso.com

### Note if sync does not occur.  On DC1 in Service > Start the Microsoft Azure AD Sync service <br<

# NOTE:  At the end of module, deallocate all the resources created in the module 

# Learnin Path 3: Implement an authentication and access management solution (~150 Miuntes)

# NOTE:  ENSURE YOU SELECT SAVE WHEN YOU FINISH THE SELECTED LABS 1-9, 12-15, 17-26 and 28

## Lab 08 – Enable multifactor authentication (~15 Minutes)

### IMPORTANT - An Azure AD Premium license is required for this exercise. - O365 AAD has already been provisioned

### Exercise 1 - Review and enable Multi-factor Authentication in Azure

Task 2 - Setup conditional access rules for MFA for Delia Dennis<br>
Step 5:  Select "Select resources" not None - Click Select - Choose Office 365<br>
Step 6:  Select Network - Choose yes on slider<br>
Step 9:  Typo - should read as Ensure that Require all the selected controls is selected<br>

## Lab 09 – Configure and deploy self-service password reset (~15 Minutes)

### Exercise 1 - Create a group with SSPR enabled and add users to it

Task 3 - Register for SSPR with Alex<br>
Step 4:  Click on Security info > + Add sign-in method <br>

## Lab 10 – Azure AD Authentication for Windows and Linux Virtual Machines (~30 Minutes)

### Exercise 1 - Login to Windows Virtual Machines in Azure with Azure AD

Task 1 - Create a Windows Virtual Machine with Azure AD login enabled<br>
Step 1: Use User 1 for the credentials <br>
Step 3: Type Windows 11 - Press Enter > Select Create in the Window 11 Box > choose Windows 11 Enterprise, version 22H2 from the menu that opens <br>
Step 3: You may have to select all sizes first to pick the DC1s_v3<br>
Step 3: Check I confirm I have an elegible Windows 10/11 license with multi-tenant hosting rights<br>

Task 2 - Microsoft Entra ID login for existing Azure Virtual Machines<br>
Read through - due to permissions you can not make any changes<br>

Task 3 - Update the Virtual Machine to allow the Microsoft Entra ID login<br>
Step 7:  Select Next > Select Accept <br>

Task 4 - Modify your RDP file to support the Microsoft Entra ID login <br>
Step 3: Ensure you choose just once when opening the file with notepad <br>

Task 6 - Optional testing to explore the Microsoft Entra ID login <br>
Step 1: User AzureAD User2 not JoniS <br>
Step 4: User AzureAD User2 not JoniS <br>
Step 8: Log on with Joseph-xxxxxx (replace xxxxx with the numbers in your user2 account) - you may have to change the password before attempting  <br>

### Optional Exercise 2 - Login to Linux Virtual Machines in Azure with Microsoft Entra ID

Task 1 - Create a Linux VM with system assigned managed identity <br>
Step 4: You may have to select all sizes first to pick the D2s_v3<br>
Step 4: There is no Password > create a Key pair name <br>

## Lab 11 - Assign Azure resource roles in Privileged Identity Management (~10 Minutes)

### Exercise 1 - PIM with Azure resources
Task 1 - Assign Azure resource roles<br>
Step 1: Credentials are located under Resources tab<br>
Skip steps 8 - 16 <br>

Task 2 - Update or remove an existing resource role assignment <br>
Step 5: On the Active assignments tab, in the Action column, review the available options <br>
Step 6: Under LOD Contributer Select User1-xxxxxx, Select Remove <br>

## Lab 12 – Manage Azure AD smart lockout values (5 Minutes)

### No Errata

## Lab 13 – Implement and test a conditional access policy (~30 Minutes)

### Exercise 1 - Set a conditional access policy to block DebraB from accessing Sway

Task 1 -- Confirm DebraB has access to Sway <br>
Debra's password is the User password not the Admin password <br>

## Lab 14 – Enable sign in and user risk policies (~10 Minutes)

### No Errata 

## Lab 15 – Configure an Azure AD multi-factor authentication registration policy (10 Minutes)

### No Errata

## Lab 16 – Using Azure Key Vault for Managed Identities (~20 Minutes)

### Exercise 1 - Use Azure Key Vault to manage Virtual Machine identities

Task 1 - Create a Key Vault<br>
Step 1:  Credentials are located on the Resources drop down<br>

Task 2 - Create a Windows Virtual Machine<br>
Step 2: Type Windows 11 - Press Enter > Select Create in Window 11 Box > Select Windows 11 Enterprise, version 23H2 from the menu that opens <br>
Step 3: Use the following setting on the Basic tab<br>
Step 3: You may have to select all sizes first to pick the D2s_v3<br>
Step 3: Confirm you have a license <br>

Task 3 - Create a secret <br>
Step 5: Leave the Name and Secret as is <br>

Task 5 - Access data with Key Vault secret with PowerShell <br>
Step 1: After logging in > Select Next > Select Accept <br>
Steps 2 - 6:  PowerShell in the RDP session - you may have to paste into notepad first <br>
# NOTE:  At the end of module, remove all policies.  Delete all the resources created in the module

# Learning Path 4: Implementing access management for apps (~90 Minutes)(Actual time ~120 Minutes)

## Lab 17 – Defender for Cloud Apps application discovery and enforcing restrictions (10 Minutes)

### Exercise 1 - Defender for Cloud Apps discovery<br>

Task 1 - Discovery apps in Defender for Cloud Apps<br>
If this is the first time accessing the Cloud App Catalog it will take 3 - 5 minutes to prepare the data <br>

## Lab 18 – Defender for Cloud Apps Access and Session Policies (20 Minutes)

### Exercise 1 - Create and test the Conditional Access App Contol policy

Task 3 - Log into Forms and validate that conditional access is monitoring<br>
Step 5: Log out and back into Microsoft Forms to see warning <br>

### Exercise 2 - Setup alerts in Microsoft Defender for Cloud Apps

Task 1 - Access Microsoft Defender for Cloud Apps and create Conditional Access App Control<br>
Step 3: If needed expand Cloud Apps in he navigation pane<br>
Step 4: Expand Policies <br>
Step 4: Select Policy Management<br>

## Lab 19 – Register an application (30 Minutes)

### Exercise 1 - Register an application

Task 2 - Configure platform settings<br>
Step 1: Click All applications then Demo App <br>

Task 3 - Add credentials, certificate and client secret <br>
Step 1: Click All applications then Demo App <br>

## Lab 20 – Implement access management for apps (5 Minutes)

## No Errata

## Lab 21 – Grant tenant-wide admin consent to an application (15 Minutes)

### Exercise 1 - Admin Consent

Task 1 - Grant admin consent in App registrations <br>
Step 1: Click All applications then Demo App <br>

# NOTE:  At the end of module, remove any policies or security settings.  Delete all the resources created in the module
 
# Learning Path 5: Plan and implement an identity governance strategy (~130 Minutes)

## Lab 22 – Create and manage a catalog of resources in Azure AD entitlement management (15 Minutes)

Task 5 - Create Access reviews for guest users <br>
Step 4: Select Teams + Groups then All Microsoft 365 groups with guests <br>
Step 5: Verify Guest users only is selected <br>
Step 9: Select weekly <br>

## Lab 23 – Add terms of use and acceptance reporting (20 Minutes)

### Exercise 1 - Set up a Term of Use and test them

Task 1 - Add terms of use<br>
Continued Task 1 - Create the Conditional Access Policy <br>
Step 8: Select the name you chose to call your ToU document <br>

## Lab 24 – Manage the lifecycle of external users in Azure AD identity Governance settings (5 Minutes)

### Exercise 1 - Microsoft Entra Identity Governance settings

Task 1 - Manage the lifecycle of external users in Microsoft Entra Identity Governance settings <br>

Step 3: In the left navigation menu, under Entitlement management, select Control configuration <br>
Step 4: In the Lifecycle of external users box, select view settings <br>
Step 5: In the lifecycle of external users section, review the different settings for external users <br>
Step 6: When an external user loses their last assignment to any access packages, if you want to block them from signing in to this directory, check the box Block external user from signing in to this directory <br>
Step 8: Once an external user loses their last assignment to any access packages, if you want to remove their guest user account in this directory, Check the box Remove external user <br>

## Lab 25 – Create Access Reviews for Internal and External Users (5 Minutes)

### Lab is an explore lab

### No Errata

## Lab 26 – Configure Privileged Identity Management for Microsoft Entra roles (30 Minutes)

### No Errata

## Lab 27 – Microsoft Sentinel Kusto Queries for Azure data sources (30 Minutes)

### Exercise 1 - Configure Microsoft Sentinel for Kusto Queries

Task 1 - Create a Microsoft Sentinel workspace<br>
Step 9: Browse back to Sentinel, click + Create, select the Workspace you created, click Add <br>

## Lab 28 – Monitor and manage security posture with Identity Secure Score (15 Minutes)

### Exercise 1 - Using Identity Secure Score to monitor and manage identity security posture

Task 2 - Execute an improvement action<br>
Skip steps 1 and 2 <BR>
Step 3: Portal does not open in correctly in new tab.  Browse to the following Entra ID > Identiy Secure Score > Identity Protection > Sign-in Risk Policy<br>

# NOTE:  At the end of the module, remove any policies or security settings.  Delete all the resources created in the module
