<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Post Installation Configurations</h1>

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- osTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- Azure Virtual Machine (VM) environment (Windows 10 4 vCPUs Recommended)

<h2>Configuration & Setup</h2>

- Before we begin, there are two panels to determine what type of user you are.
- Agent and Admin Panel. The Version you are on will show the opposing version on the top right
- In this Example here, I am logged in as an admin because it states agent panel for me to click on and go to.

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/928767fd-06a5-4a00-872b-38f24d8ef6b6)

- Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. An unlimited number of roles can be created and assigned to Agents with access to various departments.
- In the admin panel, click Agents on the top line and then roles on the next line down. From there click the + Add New Role

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/571511ab-a312-45a7-82a5-121b78ab8647)

- For this demonstration I created a role titled "Unlimited Power" check marking every box under the Tickets, Task, and Knowledge tabs. This gives this role all permissions and essentially total control, hence "Unlimited Power"

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/3c73490a-126e-41df-9c10-2c4d3bf95036)

- Departments are used to route Tickets
- While still on the previous page (Agents tab) Click departments and click + Add New Department
- Name the new deparment System Administrators and click Create Dept

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/a63af397-9ad2-4c1f-bcd5-d99c3c17614a)

- Next Create a Team and Configure it to allow anyone to create a Ticket
- In The Agents tab, Click Teams and click + Add New Team
- Create a New Team and name it (Example Tier II Support) Click Create Team

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/e9c87aea-81c4-4dad-8a1e-d5484594591e)

<h2>Creating New Agents/Users</h2>

- While Still in the Admin Panel, Click Agents on the top line followed by + Add New Agent
  
![image](https://github.com/Velezdrv/post-install-config/assets/147437260/82fc4f7f-89b1-429d-9f8f-569f2a203b01)

- Next Create two new Agents (Example Brad Pitt, Matt Damon) 

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/fedbfea1-99e8-46c8-997a-3c7814c036ba)

- Make sure to uncheck the box requiring the agent to reset the password via email and to change the password at next login.

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/1e5396da-1010-4c1a-b440-a03c750bd459)

- In the Access Tab, set the Primary Department for the Agent and their role (The ones we created earlier System Administrators/unlimited Power)
  * Side note, if we didnt use a primary that had all access, you can choose a main department and extended access for users who work in multiple departments or need access 
    to them
![image](https://github.com/Velezdrv/post-install-config/assets/147437260/3f5172dc-7e00-466f-ae5b-67cbcf9daade)

- Now add the Agent to a team, This can be used for pulling agents from multiple departments into an A team. For This we chose the Tier II support we created earlier.

![image](https://github.com/Velezdrv/post-install-config/assets/147437260/abfb4613-33a5-41b0-a108-07d18f82764e)






<h3 align = "right">Next Tutorial - <a href = "https://github.com/Velezdrv/post-install-config/tree/main">osTicket: Post Installation Configurations</a></h3>
