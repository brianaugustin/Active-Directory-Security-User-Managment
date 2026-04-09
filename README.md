## Active-Directory-Security-User-Managment
### Primary objective was to enforce strict identity management and data exfiltration prevention through two main avenues:

Password Hardening: I designed and deployed a custom Password Policy GPO that enforces a 12-character minimum length, 90-day expiration cycle, and mandatory complexity requirements (uppercase, lowercase, numbers, and symbols). This mitigates the risk of credential-based attacks like brute-forcing and password spraying.

Endpoint Security: I configured a USB Device Restriction policy to disable unauthorized external storage. This is a critical security measure to prevent data theft and the introduction of malware or "Rubber Ducky" style hardware attacks into the network.

Directory Management: Using the Group Policy Management Console (GPMC), I managed the scope and inheritance of these policies, ensuring they were correctly linked to the domain root and targeted toward the appropriate "Authenticated Users" and Organizational Units (OUs).

![Group Policy Management Editor Overview](https://github.com/user-attachments/assets/2f58050a-b932-4563-8616-d0ab1842563c)
![Configuring Password Expiration and Complexity](https://github.com/user-attachments/assets/fbf8c819-6019-4e93-8ff2-3fec74a04d9c)
![Setting Minimum Password Length](https://github.com/user-attachments/assets/0800ae81-2f03-4705-a63a-3032f6bc97a2)
![Creating a New Group Policy Object](https://github.com/user-attachments/assets/d06d4bb6-9de6-47a6-9c1f-71ab481f99d1)
![Group Policy Management Editor Overview-2](https://github.com/user-attachments/assets/653fd212-ba4b-44bb-a42a-6f162a4ea497)
