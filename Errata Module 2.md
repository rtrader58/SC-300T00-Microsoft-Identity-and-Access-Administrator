# SC-300T00 Microsoft Identity and Access Administrator - Module 2 Errata

# NOTE: ENSURE YOU SELECT SAVE WHEN YOU FINISH THE SELECTED LABS 1-9, 12-15, 17-26 and 28

# Module 2: Implement an identity management solution (~120 Minutes)

# Optional - Lab 07 - Cannot be accomplished in the current environment - requires creating a trial subscription
Important note: Lab requires a time-consuming deployment. <br>

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

Task 3 - Add an Office license to sg-SC300-O365
Step 9: Should read sf-SC300-0365 not Raul

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

Task 1- Configure Google to be used as an identity provider<br>
Note:  Create a Gmail account for use in this lab, I recommend something like this<br>
Initialssc300@gmail.com (FFsc300@gmail.com)<br>
If the account is taken use a recommended one – Note your username and password<br>

Step 1:  Does not paste – type in manually<br>
Step 13: Copy and paste the URLs into notepad, paste 1 line at a time do not include the – <br>
Step 14: Copy the client ID and Secret and paste in notepad<br>

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

 

