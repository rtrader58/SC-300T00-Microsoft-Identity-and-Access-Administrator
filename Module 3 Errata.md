# SC-300T00 Microsoft Identity and Access Administrator - Module 3 Errata

# NOTE:  At the end of each module of labs, delete all the resources created in the module

## Implement an authentication and access management solution (~150 Miuntes)

## Lab 08 – enable Azure AD multifactor authentication (15 Minutes)

### IMPORTANT - An Azure AD Premium license is required for this exercise. - O365 AAD has already been provisioned

### Exercise 1 - Review and enable Multi-factor Authentication in Azure

Task 2 - Setup conditional access rules for MFA for Delia Dennis
Step 9:  Typo - should read as Ensure that Require all the selected controls is selected

## Lab 09 – Configure and deploy self-service password reset (15 Minutes)

### Exercise 1 - Create a group with SSPR enabled and add users to it

Task 3 - Register for SSPR with Alex<br>
Step 4:  Click on Security info > + Add sign-in method <br>

## Lab 10 – Azure AD Authentication for Windows and Linux Virtual Machines (30 Minutes)

### Exercise 1 - Login to Windows Virtual Machines in Azure with Azure AD

Task 1 - Create a Windows Virtual Machine with Azure AD login enabled<br>
Use the following setting on the Basic tab<br>
Resource group;  myDemoRG<br>
Virtual machine name:  myVM1<br>
Availability options:  No infrastructure redundancy required<br>
Image:  Windows Server 2019 Datacenter – Gen 1<br>
Username:  demouser<br>
Password:  demo@pass123<br>

On the Management tab, check the box to Login with Azure AD under the Azure AD section.<br>
Make sure System assigned managed identity under the Identity section is checked. This action should happen automatically once you enable Login with Azure AD.<br>

Task 2 - Azure AD login for existing Azure Virtual Machines<br>
Step 4:  Choose your Global Admin as a member<br>

### Exercise 2 - Login to Linux Virtual Machines in Azure with Azure AD

Task 1 - Create a Linux VM with system assigned managed identity<br>
Use the following setting on the Basic tab<br>
Resource group;  myDemoRG<br>
Virtual machine name:  myVM2<br>
Availability options:  No infrastructure redundancy required<br>
Authentication type:  Password<br>
Username:  demouser<br>
Password:  demo@pass123<br>

On the Management tab, check the box to Login with Azure AD under the Azure AD section.<br>
Make sure System assigned managed identity under the Identity section is checked. This action should happen automatically once you enable Login with Azure AD.<br>

Task 2 - Azure AD login for existing Azure Virtual Machines<br>
Step 4:  Choose your Global Admin as a member<br>

## Lab 11 - Assign Azure resource roles in Privileged Identity Management (10 Minutes)<br>

### No errata

## Lab 12 – Manage Azure AD smart lockout values (5 Minutes)

### No Errata

## Lab 13 – Implement and test a conditional access policy (30 Minutes)

### No Errata

## Lab 14 – Enable sign in and user risk policies (10 Minutes)

### No Errata 

## Lab 15 – Configure an Azure AD multi-factor authentication registration policy (10 Minutes)

### No Errata

## Lab 16 – Using Azure Key Vault for Managed Identities (20 Minutes)

### Exercise 1 - Use Azure Key Vault to manage Virtual Machine identities

Task 1 - Create a Windows Virtual Machine with Azure AD login enabled<br>
Use the following setting on the Basic tab<br>
Resource group;  myDemoRG<br>
Virtual machine name:  myVM3<br>
Availability options:  No infrastructure redundancy required<br>
Image:  Windows Server 2019 Datacenter – Gen 1<br>
Username:  demouser<br>
Password:  demo@pass123<br>

On the Management tab, check the box to Login with Azure AD under the Azure AD section.<br>
Make sure System assigned managed identity under the Identity section is checked. This action should happen automatically once you enable Login with Azure AD.<br>

Task 2 - Create a Key Vault<br>
Step 6:  May need to add your initials to the Key vault name<br>

Task 5 - Access data with Key Vault secret with PowerShell<br>
Step 2: returns unable to resolve the name.  Open a PowerShell Prompt.  Use IP config to determine the computer’s IP address.  Replace the address in the CMDLET with the IP address<br>

# NOTE:  At the end of module, remove all policies.  Delete all the resources created in the module
