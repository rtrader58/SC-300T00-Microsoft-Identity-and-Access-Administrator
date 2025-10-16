# SC-300T00 Microsoft Identity and Access Administrator - Learning Path 3 Errata

# NOTE: ENSURE YOU SELECT SAVE WHEN YOU FINISH THE SELECTED LABS 1-9, 12-15, 17-26 and 28

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

# NOTE:  ENSURE YOU SELECT SAVE WHEN YOU FINISH THE SELECTED LABS

