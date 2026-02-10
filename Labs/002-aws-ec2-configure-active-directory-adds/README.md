# active-directory-vm-lab

A beginner-friendly lab that installs and configures Active Directory Domain Services (AD DS) on a Windows Server virtual machine, then performs basic user administration in Active Directory.

## Watch me build this lab
loom.com/share/3edd30f8c1a948e2b4d482b8c217c1c4

**What this video shows:** Installing AD DS, promoting a server to a Domain Controller, and creating a test user in Active Directory Users and Computers.

---

## Objective
Stand up a simple Active Directory domain on a Windows Server VM and validate it by managing directory objects.

---

## Skills Practiced
- Installing Windows Server roles and features
- Configuring Active Directory Domain Services (AD DS)
- Promoting a server to a Domain Controller
- Creating a new forest and domain (example: school.local)
- Navigating Active Directory Users and Computers (ADUC)
- Creating and managing users in Active Directory
- Understanding Organizational Units (OUs) at a high level
- Reconnecting to a server after role installation/reboot

---

## Tools Used
- Windows Server virtual machine
- Server Manager
- Active Directory Domain Services (AD DS)
- Active Directory Users and Computers (ADUC)
- Remote Desktop (RDP)

---

## Steps Performed
1. **Open Server Manager**  
   Launched Server Manager to begin adding server roles and features for directory services.  
   (Optional screenshot) docs/step-1.png

2. **Start Add Roles Wizard**  
   Initiated the “Add Roles and Features” workflow to install the required server role.  
   (Optional screenshot) docs/step-2.png

3. **Install Active Directory Domain Services**  
   Selected and installed the AD DS role (including required features) on the server.  
   (Optional screenshot) docs/step-3.png

4. **Promote Server to Domain Controller**  
   Promoted the server to a Domain Controller and created a new forest/domain (example: school.local).  
   (Optional screenshot) docs/step-4.png

5. **Complete Promotion and Reconnect**  
   Completed the installation, allowed the server to restart/log out, and reconnected back into the VM.  
   (Optional screenshot) docs/step-5.png

6. **Open Active Directory Users and Computers**  
   Verified AD tools were available and opened ADUC to manage the new domain directory structure.  
   (Optional screenshot) docs/step-6.png

7. **Create a Test User and Review OUs**  
   Created a sample user account and reviewed how Organizational Units can be used to organize and manage users.  
   (Optional screenshot) docs/step-7.png

8. **Verify Functionality**  
   Confirmed the domain and directory objects were accessible and changes (like the new user) appeared as expected.  
   (Optional screenshot) docs/step-8.png

---

## Outcome
Active Directory was successfully installed and configured on the VM, and basic administration was validated by creating and viewing directory objects in ADUC.
