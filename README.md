<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Configure and promote DC-1 as a Domain Controller.
- Configure a Domain Admin user and create Organizational Units (OUs).
- Join Client-1 to the domain.
- Verify and organize Client-1 in Active Directory Users and Computers (ADUC).

<h2>Deployment and Configuration Steps</h2>

<img width="1728" alt="image" src="https://github.com/user-attachments/assets/46e81971-5f0c-4468-b0c7-8b78df60c228" />

- Add active directory and create own root domain by choosing (add new forest) then, proceed to install.

<img width="1728" alt="image" src="https://github.com/user-attachments/assets/b0098e36-3370-4d5c-8d07-a4bbf370cbcb" />

- On here we should create Organizational unit ( _EMPLOYEES & _ADMINS) and create a user within _Admins file (jane doe)

<img width="1728" alt="image" src="https://github.com/user-attachments/assets/f00826ff-dbdf-4055-b0c8-617c696c9220" />

- We must add jane "the user" to domain admins security group that was created earlier in order to gain control.

<img width="1728" alt="image" src="https://github.com/user-attachments/assets/8d3eda57-b9ee-42d3-81cc-de9ab23e88d1" />

- Here, we allow the client-1 account to join to the dc-1 domain.

<img width="1728" alt="image" src="https://github.com/user-attachments/assets/53b83ea5-1e1d-4d1a-982f-1609dde71cab" />

- Finally, we organize client-1 in Active Directory and move it to the (_clients) file
