# Project: Active Directory Identity and Data Security

I implemented a set of Group Policy Objects (GPOs) to strengthen identity management and prevent unauthorized data transfers within a Windows Domain environment. This project focuses on two critical security areas: hardening user credentials and restricting physical data exfiltration points.

Project Scope
The goal was to move beyond default security settings by enforcing stricter password requirements and locking down hardware endpoints. By managing these through the Group Policy Management Console (GPMC), I ensured that these security controls are automatically applied to all users and workstations joined to the domain.

## Active Directory Password Policy Configuration

I configured a custom Password Policy within a Windows Server environment using Active Directory and Group Policy Objects (GPOs). My goal was to enforce stronger security requirements for all users in the domain.

## Project Steps

### 1. Navigating to the Management Console
I started by opening the Group Policy Management tool. I needed to locate the specific domain where the policy would be applied. In the image below, I am navigating the forest and domain structure to find the Default Domain Policy.

<img src="https://github.com/user-attachments/assets/2f58050a-b932-4563-8616-d0ab1842563c" width="600">

### 2. Accessing the Password Policy Folder
Once I opened the editor for the domain policy, I drilled down through the Computer Configuration settings. I went into Policies, then Windows Settings, and finally Security Settings. I have selected the Password Policy folder to view the current active rules.

<img src="https://github.com/user-attachments/assets/fbf8c819-6019-4e93-8ff2-3fec74a04d9c" width="600">

### 3. Defining Minimum Password Length
I increased the minimum password length to ensure better security. I opened the Minimum password length setting and changed the value to 7 characters. The image shows the properties window where I defined this requirement.

<img src="https://github.com/user-attachments/assets/0800ae81-2f03-4705-a63a-3032f6bc97a2" width="600">

### 4. Creating a New Policy Object
I also practiced creating a separate Group Policy Object. This allows for more control when applying rules to specific groups. Here, I am right-clicking the domain to create a new GPO and link it.

<img src="https://github.com/user-attachments/assets/d06d4bb6-9de6-47a6-9c1f-71ab481f99d1" width="600">

### 5. Verifying the Final Configuration
Finally, I returned to the Group Policy Management Editor to verify that all changes were saved. The image displays the updated list of security settings, confirming that complexity, history, and length are now enforced.

<img src="https://github.com/user-attachments/assets/653fd212-ba4b-44bb-a42a-6f162a4ea497" width="600">
