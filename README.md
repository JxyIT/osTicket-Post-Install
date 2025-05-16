<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Roles
- Departments and Teams
- Agents and Users
- SLA and Help Topics

<h2>Configuration Steps</h2>

Acknowledge Agent Panel vs Admin Panel

Configure Roles (for grouping permissions)
Admin Panel -> Agents -> Roles
Supreme Admin
![image](https://github.com/user-attachments/assets/f995c3ac-7403-446a-b357-59607f9120f7) ![image](https://github.com/user-attachments/assets/f6df411b-b401-4d93-ae61-5ddbb23bc9fb)

Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
Admin Panel -> Agents -> Departments
SysAdmins
![image](https://github.com/user-attachments/assets/1ddd05b3-51ae-4b0e-92ed-42af9b6588ff)

Configure Teams
Admin Panel -> Agents -> Teams (Pull Agents from different Departments)
Online Banking
![image](https://github.com/user-attachments/assets/6fae3e7b-e056-4ab6-96c8-5a122bfd442b)


Allow anyone to create tickets
Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)
Registration Required: Registration and login are required to create tickets 
![image](https://github.com/user-attachments/assets/1a02750e-40e3-4181-8328-321f8980688e)


Configure Agents (workers)
Admin Panel -> Agents -> Add New
Jane (Dept: SysAdmins)
John (Dept: Support)
![image](https://github.com/user-attachments/assets/94779418-1aba-4612-93f9-540454f22541)

Configure Users (customers)
Agent Panel -> Users -> Add New
Karen
![image](https://github.com/user-attachments/assets/bf82e2bf-ba70-4824-829b-bfab5397e3c0)

Configure SLA
Admin Panel -> Manage -> SLA
Sev-A (Grace Period: 1 hour, Schedule: 24/7)
Sev-B (Grace Period: 4 hours, Schedule: 24/7)
Sev-C (Grace Period: 8 hours, Business Hours)
![image](https://github.com/user-attachments/assets/cbc91d30-c998-426b-9beb-d64b20e4a8a7)

Configure Help Topics (For when users create a ticket)
Admin Panel -> Manage -> Help Topics,
Business Critical Outage,
Personal Computer Issues,
Equipment Request,
Password Reset,
Other
![image](https://github.com/user-attachments/assets/c37c88e1-8d19-429b-8d6d-ffd084caf2d0)

