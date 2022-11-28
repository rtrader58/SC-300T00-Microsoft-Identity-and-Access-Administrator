# SC-300T00 Microsoft Identity and Access Administrator - Modules 2 Errata<br>

# NOTE:  At the end of each module of labs, delete all the resources created in the module<br>

# Implement an identity management solution (~190 Minutes)<br>

## Lab 0 - Create a Microsoft Azure Pass Subscription (10 Minutes)<br>
Step 2:  Activate your subscription<br>
Leave Name and email as is, enter your information in the remaining fields – must include a valid phone number and address<br>

# Disregarrd - Read this at the very end of Lab 0:<br> 

# Disregarrd - Lab 07 has been removed from the environment. - Go straight to Lab 01<br>

Important note: a later lab requires a time-consuming deployment. To save your time later, we suggest that you kick off that portion of the lab now so it’s ready when you get there. To do that:<br>

After completing Lab 0 use the next button to skip to Lab 07.  Complete Lab 07 Exercise 1 Task 1 - Once the deployment has started use the previous button to return to Lab 01 Continue with Lab 01, and Lab 07 should be ready when you get there<br>

## Lab 01 – Manage user roles (30 Minutes)
<br>

### Exercise 1 – Create a new user and test their application admin rights

<br>

Task 1:  Add a new user<br>
Step 6:  Use the following password<br>
Pass@word!<br>

Task 2: Bulk addition of users using PowerShell<br>
Step 2: After running Install-Module AzureAD run Import-Module AzureAD to import the module prior to use<br><br>

<br>

### Exercise 4 - Bulk import of users

<br>

Task 1 - Bulk operations for creating users with a .csv file<br>
Step 6:  After opening the .csv file paste your tenant name from the resources tab in the lab guide at the bottom of the file<br>
Use the replace feature in Notepad to replace <<<enter your domain name>>><br>
After pasting delete your tenant name you pasted at the bottom of the file <br>

Task 2:  Bulk addition of users using PowerShell<br>

Step 7:  Copy and paste your tenant name from the Azure Portal notepad<br>
Paste the New-Aduser cmdlet into notepad<br>
Replace the labtenname.com with your tenant name<br>
Copy and paste cmdlet into PowerShell<br>

<br>

### Exercise 6 - Add a Windows 10 license to a user account

<br>

Task 1 - Find your unlicensed user in Azure Active Directory<br>
Step 5:  Click edit properties > Settings tab to verify Usage location<br>

<br>

## Lab 02 – Working with tenant properties (15 Minutes)

<br>

### Exercise 3 - Setting your privacy information

<br>

Task 1 - Adding your privacy info on Azure AD, including Global privacy contact and Privacy statement URL<br>
Step 2:  Will not paste.  In the lab environment use edge to browse to the github.com repository to the pdf and copy URL from browser<br>
Use the following steps to get to the PDF<br>
https://github.com <br>
On the github page search for SC-300<br>
Select MicrosoftLearning > Allfiles > Labs > Lab2 > SC-300-Lab_ContosotPrivacySample.pdf<br>
Copy URL<br>

<br>

## Lab 03:  Assigning licenses using group membership (25 Minutes)

<br>

Exercise 1 - Create a security group and add a user<br>
Task 4 - Confirm the SteOffice 365 license<br>
Step 4:  it may take up to 5 minutes for the license to be applied, logout wait a few minutes log back in<br>

<br>

## Lab 04:  Configure external collaboration settings (5 Minutes)

<br>

### No errata

<br>

## Lab 05 -Add guest users to the directory (5 Minutes)

<br>

### Exercise 1 – Add guest user to the directory

<br>

Step 4:  Use the New user drop down box, select Invite external user<br>

<br>

### Exercise 2 - Invite guest users in bulk<br>

<br>

Task 1 - Bulk user invite<br>
Use the step as an example, do not actually submit the file<br>

Task 2 - Invite guest users with PowerShell<br>
PowerShell was installed in a previous lab you may be able to start at step 4<br>

<br>

## Lab 06 – Add a federated identity provider (25 Minutes)

<br>

### Exercise 1 – Configure identity providers

<br>

Task 1- Configure Google to be used as an identity provider<br>
Note:  Create a Gmail account for use in this lab, I recommend something like this<br>
Initialssc300@gmail.com (FFsc300@gmail.com)<br>
If the account is taken use a recommended one – Note your username and password<br>

Step 1:  Does not paste – type in manually<br>
Step 5:  In the Application type menu, select Web application. Give the application a suitable name, like Azure AD B2B. Under Authorized redirect URIs, add the following URIs:<br>
Copy and paste the URLs into notepad, paste 1 line at a time do not include the – <br>
Copy the client ID and Secret and paste in notepad<br>

<br>

# Disregarrd - Lab 07 has been removed from the environment.

## Lab 07 – Add Hybrid Identity with Azure AD Connect (75 Minutes)

<br>

### Exercise 1 – Setup On-Premises infrastructure

<br>
Task 1 – Create the on-premises Active Directory infrastructure<br>
Step 1:  The link may not paste in the lab environment, if not enter the following in Edge<br>
	https://github.com/maxskunkworks/TLG/tree/master/tlg-base-config_3-vm<br>
Step3:  when deplying the VM choose size  Standard_D2s_v2<br>

Note the DNS label prefix you use – I used retSC300<br>
Note:  If you jumped here after completing Lab 0, do not wait for the deployment to finish, press Previous to return to Lab 1<br>

Task 2 - Configure the lab environment Azure VMs<br>
Step 1:  Password is incorrect use   demo@pass123<br>
Steps 2, 3, 4, 5 it easier to run each one in a separate tab in the PowerShell ISE<br>

There is no Task 4<br>

Task 5 - Configure contoso.local Active Directory<br>
Step 1:  Password is incorrect use   demo@pass123<br>
After connecting, launch IE download and install Chrome.  Then complete task 5 in Chrome<br>
Replace Step 2 with the following: <br> 
Browse to https://github.com/microsoft/MCW-Hybrid-identity<br>
Select the Code box and click on Download zip.<br>
Browse to the downloaded file and extract<br>
Browse to c:downloads\MCW-hybrid-identity-main\ MCW-hybrid-identity-main\Hands-on labs\studentfiles<br>
Skip to Step 5<br>
Step 8:  After running the script open Active Directory Users and Computers to verify the Demo Accounts OU has been created and populated with users and groups.<br>

Note:  when the script is running you may see red flashing by, ignore<br>
Do not run the script a second time, it will delete the Demo Accounts OU<br>
Step 9:  Paste into another tab in the ISE before running<br>
Step 10:  Paste into another tab in the ISE before running<br>

<br>

### Exercise 2: Integrate an Active Directory forest with an Azure Active Directory tenant

<br>

Task 1: Create an Azure Active Directory tenant and activate an EMS E5 trial<br>
Step 6:  recommend initials then Contoso when creating the initial domain name<br>

Note:  do not close the Captia once it says Tenant Creation in Progress<br>
Step 7:  Select navigate to tenant when successful<br>
Skip to Step 11<br>

Task 3: Purchase a custom domain name<br>
Step 1:  Navigate to Azure Active Directory > Manage tenants > Select the Contoso Marketing Tenant > Switch <br>
Skip Step 2<br>
Step 9:  change the email to a valid email you use<br>
Step 12:  If deployment fails continue with the next task.<br>
Your custom domain name will not verify but the lab will still work<br>
Task 6: Install Azure AD Connect<br>
Step 18:  Password is demo@pass123<br>
Step 25:  Password is demo@pass123<br>
Task 9: Initiate and verify directory synchronization<br>
Step 11:  In Chrome<br>
Task 11: Perform Hybrid Azure AD join<br>
Step 3;  Login as  corp\AGAyers<br>

<br>

# NOTE:  At the end of module, delete all the resources created in the module
 

