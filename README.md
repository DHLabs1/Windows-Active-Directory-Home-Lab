# Active Directory Home Lab (Cybersecurity Focus)

## Overview
This project demonstrates the setup and configuration of a Windows Active Directory environment
using VirtualBox. The lab simulates an enterprise domain environment commonly encountered in
help desk and SOC roles.

## Technologies Used
- VirtualBox
- Windows Server 2025
- Windows 11 Enterprise
- Active Directory Domain Services (AD DS)
- DNS & DHCP
- PowerShell
- Group Policy

## Lab Architecture
- Domain Controller with dual NICs (NAT + Internal Network)
- Windows 11 client joined to the domain
- Isolated internal network for AD communication

## Key Skills Demonstrated
- Active Directory installation and domain promotion
- DNS and DHCP configuration
- Organizational Units (OUs) and Group Policy
- User and group management
- PowerShell automation for bulk user creation
- Windows domain joining and troubleshooting

**1. Installing Active Directory Domain Services (AD DS)**


![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/ea4eb02ef09b4a6882e8b3eab480d822a150a8c3/screenshots/Installing%20Active%20Directory%20Domain%20Services%20(AD%20DS).JPG)  


**Description:**  
This screenshot shows the Add Roles and Features Wizard during the installation of the Active Directory Domain Services (AD DS) role on Windows Server. The system prompts to add required features needed to support Active Directory functionality.

**Key Actions Performed:**
- Selected Active Directory Domain Services from Server Roles
- Installed required supporting features
- Enabled Group Policy Management

**Skills Demonstrated:**
- Windows Server role installation
- Active Directory infrastructure setup
- Identity and Access Management (IAM) fundamentals


**2. Promoting the Server to a Domain Controller**


![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/694ffdc944582f04fc95bae263683f416855711e/screenshots/Promote%20Server%20to%20Domain%20Controller.JPG)

Description:
This screenshot shows Server Manager after the AD DS role installation, displaying the post-deployment configuration warning prompting the administrator to promote the server to a domain controller.

Key Actions Performed:
- Verified successful installation of AD DS role
- Initiated post-deployment configuration
- Selected the option to promote the server to a Domain Controller

Skills Demonstrated:
- Server Manager administration
- Active Directory deployment workflow
- Understanding of domain controller responsibilities

**3. Creating a New Forest and Domain**

Screenshot:
Domain Controller - Add New Forrest.JPG

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Domain%20Controller%20-%20New%20Forrest%20Creation.JPG)

Description:
This screenshot shows the Active Directory Domain Services Configuration Wizard during deployment configuration, where a new forest is created with a custom root domain name.

Key Actions Performed:
- Selected Add a new forest
- Defined the root domain name: DHLabs.com
- Prepared the environment for a new Active Directory domain structure

Skills Demonstrated:
- Active Directory forest and domain design
- Enterprise identity architecture
- Secure directory service configuration

**4. Organizational Unit (OU) and User Creation**

Screenshot:
OU and User Creation.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/OU%20and%20User%20Creation.JPG)


Description:
This screenshot shows the creation of Organizational Units (OUs) and user accounts within Active Directory Users and Computers (ADUC). OUs are used to logically organize directory objects and apply administrative control and security policies.

Key Actions Performed:
- Created Organizational Units to separate users and resources
- Followed naming conventions consistent with enterprise environments

Skills Demonstrated:
- Active Directory object management
- Identity lifecycle management
- Role-based access control (RBAC) principles

**5. ADMINS OU Creation**

Screenshot:
ADMINS OU Creation.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/ADMINS%20OU%20Creation.JPG)

Description:
This screenshot shows the creation of a dedicated Administrators Organizational Unit (OU) within Active Directory to separate privileged accounts from standard users.

Key Actions Performed:
- Created a dedicated OU for administrative accounts
- Applied logical separation between standard and privileged users
- Followed least-privilege and tiered administration concepts

Skills Demonstrated:
- Active Directory OU design
- Privileged account management
- Enterprise security best practices

**6. Admin Group Added to Admins OU**

Screenshot:
Admin Group Added To Admins OU.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Admin%20Group%20Added%20To%20Admins%20OU.JPG)

Description:
This screenshot shows an administrative security group being created and placed inside the Admins OU for centralized privilege management.

Key Actions Performed:
- Created an administrative security group
- Placed the group within the Admins OU
- Prepared group structure for delegated permissions

Skills Demonstrated:
- Group-based access control
- Active Directory security groups
- IAM best practices

**7. Delegate Admin Permissions to Company Admin Group**

Screenshot:
Delegate Admin Permissions to Company Admin Group.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Delegate%20Admin%20Permissions%20to%20Company%20Admin%20Group.JPG)

Description:
This screenshot shows the delegation of administrative permissions to a designated Company Admin group using Active Directory delegation controls.

Key Actions Performed:
- Delegated specific administrative rights to a security group
- Avoided assigning permissions directly to user accounts
- Applied principle of least privilege

Skills Demonstrated:
- Delegation of control
- Least privilege implementation
- Active Directory administration

**8. Remote Access Service and Network Address Translation Installation**

Screenshot:
Remote Access Service and Network Address Translation Installation.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Remote%20Access%20Service%20and%20Network%20Address%20Translation%20Installation%20Part%201.JPG)


![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Remote%20Access%20Service%20and%20Network%20Address%20Translation%20Installation%20Part2.JPG)

Description:
This screenshot shows the installation of the Remote Access role, including Network Address Translation (NAT), to allow internal systems to access external networks.

Key Actions Performed:
- Installed Remote Access role
- Enabled NAT functionality
- Prepared the environment for internal-to-external connectivity

Skills Demonstrated:
- Network services configuration
- Secure network design
- Windows Server routing concepts

**9. Configure NAT for Internal Users**

Screenshot:
Configure NAT For Internal Users.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Configure%20NAT%20For%20Internal%20Users.JPG)

Description:
This screenshot shows the configuration of NAT rules allowing internal domain systems to access external networks through the domain controller.

Key Actions Performed:
- Configured NAT interfaces
- Defined internal and external network boundaries
- Enabled internet access for internal clients

Skills Demonstrated:
- Network traffic routing
- NAT configuration
- Infrastructure security fundamentals

**10. DHCP Server Installation**

Screenshot:
DHCP Server Installation.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/DHCP%20Server%20Installation.JPG)

Description:
This screenshot shows the installation of the Dynamic Host Configuration Protocol (DHCP) server role on Windows Server.

Key Actions Performed:
- Installed DHCP Server role
- Added required DHCP management tools
- Prepared server for automated IP assignment

Skills Demonstrated:
- DHCP server deployment
- Network services administration
- Windows Server management

**11. New DHCP Scope**

Screenshot:
New DCHP Scope.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/New%20DCHP%20Scope.JPG)

Description:
This screenshot shows the creation of a new DHCP scope, defining the IP address range available to client systems.

Key Actions Performed:
- Created an IPv4 scope
- Defined IP range, subnet mask, and lease duration
- Configured scope options

Skills Demonstrated:
- DHCP scope design
- IP address management
- Network configuration

**12. Authorize DHCP Scope**

Screenshot:
Authorize DHCP Scope.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Authorize%20DHCP%20Scope.JPG)

Description:
This screenshot shows the DHCP server being authorized in Active Directory, allowing it to distribute IP addresses to domain clients.

Key Actions Performed:
- Authorized DHCP server in AD
- Enabled the DHCP scope
- Verified service readiness

Skills Demonstrated:
- Active Directory integration
- DHCP security controls
- Enterprise network governance

**13. New User Generation with PowerShell Script**

Screenshot:
New User Generation With Powershell Script.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/New%20User%20Generation%20With%20Powershell%20Script.JPG)

Description:
This screenshot shows the execution of a PowerShell script to automate the creation of multiple user accounts in Active Directory.

Key Actions Performed:
- Used PowerShell to bulk-create users
- Applied consistent naming conventions
- Reduced manual administrative effort

Skills Demonstrated:
- PowerShell scripting
- Automation for IAM
- Administrative efficiency

**14. Add Client PC to Domain**

Screenshot:
Add Client PC to Domain.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Add%20Client%20PC%20to%20Domain.JPG)

Description:
This screenshot shows a Windows client system being configured to join the Active Directory domain.

Key Actions Performed:
- Configured DNS settings
- Joined client machine to the domain
- Used domain credentials for authentication

Skills Demonstrated:
- Domain integration
- Endpoint management
- Windows networking

**15. Successfully Added Client to DHLabs Domain**

Screenshot:
Successfully Added Client to DHLabs Domain.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Successfully%20Added%20Client%20to%20DHLabs%20Domain.JPG)

Description:
This screenshot confirms the successful addition of a client computer to the DHLabs.com domain.

Key Actions Performed:
- Verified domain membership
- Confirmed successful authentication
- Completed domain join process

Skills Demonstrated:
- Domain validation
- Troubleshooting
- Enterprise endpoint onboarding

**16. DHCP Server Successfully Grants Lease to Client1 PC**

Screenshot:
DHCP Server Successfully Grants Lease To Client1 PC.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/DHCP%20Server%20Successfully%20Grants%20Lease%20To%20Client1%20PC.JPG)

Description:
This screenshot shows the DHCP server successfully issuing an IP address lease to a domain-joined client.

Key Actions Performed:
- Verified active DHCP lease
- Confirmed correct IP assignment
- Ensured network connectivity

Skills Demonstrated:
- DHCP monitoring
- Network validation
- Infrastructure troubleshooting

**17. Successful Login to Domain**

Screenshot:
Successful Login To Domain.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Successful%20Login%20To%20Domain.JPG)

Description:
This screenshot shows a successful domain user login from a client machine using Active Directory credentials.

Key Actions Performed:
- Logged in using domain account
- Authenticated against domain controller
- Confirmed access permissions

Skills Demonstrated:
- Authentication validation
- Identity verification
- Access control testing

**18. Created User Confirmed Member Of Domain**

Screenshot:
Kobe Bryant Confirmed Member Of Domain.jpeg

![image alt](https://github.com/DHLabs1/Windows-Active-Directory-Home-Lab/blob/0e341087142be70fa4350cbe9bc8a42c1a3cb235/screenshots/Kobe%20Bryant%20Confirmed%20Member%20Of%20Domain.JPG)

Description:
This screenshot confirms that the user account “Kobe Bryant” exists within Active Directory and is properly recognized as a domain user.

Key Actions Performed:
- Verified user account presence in AD
- Confirmed correct OU placement
- Ensured domain membership

Skills Demonstrated:
- User account verification
- Directory auditing
- Identity management validation
