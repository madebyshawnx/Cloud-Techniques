# AWS EC2 Windows VM Lab (RDP Access)

A beginner-friendly lab that walks through launching a Windows virtual machine in AWS and connecting to it securely via Remote Desktop (RDP).

## Watch me build this lab
https://loom.com/share/9a034b9d77f143d18157d71631305b02

**What this video shows:** Launching a Windows EC2 instance, creating a key pair, retrieving the Windows password, and connecting via RDP.

---

## Objective
Create and connect to a Windows virtual machine on AWS (EC2) so you have a working remote server environment for follow-on labs.

---

## Skills Practiced
- AWS EC2 instance provisioning
- Instance sizing and free-tier awareness
- Key pair creation and secure handling
- Basic networking/security review for remote access
- Instance health checks and status monitoring
- Windows password retrieval and decryption
- Remote Desktop (RDP) connectivity
- Cost-control habits (logging out / stopping when not in use)

---

## Tools Used
- AWS Management Console
- Amazon EC2
- Windows Server EC2 instance (example: Windows)
- Key pair file (PEM)
- Remote Desktop client (RDP)

---

## Steps Performed
## Creating a Virtual Machine in AWS

### Objective

This SOP outlines the steps to create and connect to a virtual machine in AWS, ensuring team members can execute the process efficiently.

### Key Steps

**Step 1: Access AWS and Launch Instances** [0:05](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=5)

![generated-image-at-00:00:05](https://loom.com/i/fda83393c37f415db2c286af7d859a74?workflows_screenshot=true)

- Go to the side of the room and log in using your email.
- Wait for the dashboard to load.
- Click on 'Launch Instances' to start creating a new virtual machine.

**Step 2: Configure the Virtual Machine** [0:30](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=30)

![generated-image-at-00:00:30](https://loom.com/i/609898fc15e141e493a75dbec37eeffb?workflows_screenshot=true)

- Name your server (e.g., 'My Server 01').
- Select the type of virtual machine (choose Windows).
- Choose the instance type that fits within the free tier (e.g., 2 CPU, 8 GB memory).

**Step 3: Create a Key Pair** [1:25](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=85)

![generated-image-at-00:01:25](https://loom.com/i/bbc22ab6a0284f85aa2d3bffac5421ae?workflows_screenshot=true)

- Select 'Create Key Pair'.
- Name your key pair (e.g., 'MyServerKey01').
- Click 'Create Key Pair' and ensure to download and save the key file securely.

**Step 4: Configure Network Settings** [2:20](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=140)

![generated-image-at-00:02:20](https://loom.com/i/0bea35cbfafb4b97a4439a8318650268?workflows_screenshot=true)

- Leave the network settings as default.
- Click 'Launch Instance' to finalize the setup.

**Step 5: Monitor Instance Initialization** [3:10](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=190)

![generated-image-at-00:03:10](https://loom.com/i/b3a0aa14e2e5430dbe251bf27b87dd51?workflows_screenshot=true)

- Go to 'Instances' to check the status of your new virtual machine.
- Wait until the status shows '3 out of 3 checks passed'.

**Step 6: Start the Instance** [3:50](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=230)

![generated-image-at-00:03:50](https://loom.com/i/1ca8da2cfb95459f8c5f016a3d8007e3?workflows_screenshot=true)

- Select your virtual machine.
- Click on 'Instance State' and then 'Start Instance'.

**Step 7: Connect to the Instance** [4:21](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=261)

![generated-image-at-00:04:21](https://loom.com/i/29f06b2d98e2414ead7e5f65661fe347?workflows_screenshot=true)

- Once the instance is running, click on 'Connect'.
- Use the RDP client to connect.

**Step 8: Retrieve Password** [4:41](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=281)

![generated-image-at-00:04:41](https://loom.com/i/59eab177f9b441e08461e3771a4fad7f?workflows_screenshot=true)

- Click on 'Get Password'.
- Upload the private key you downloaded earlier.
- Click 'Decrypt Password' and copy the generated password.

**Step 9: Download Remote Desktop File** [5:07](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=307)

![generated-image-at-00:05:07](https://loom.com/i/2e209302e3b14dc989e85f1b45e707c4?workflows_screenshot=true)

- Click on 'Download Remote Desktop File'.
- Open the downloaded file and enter the password when prompted.

**Step 10: Access the Virtual Machine** [5:44](https://loom.com/share/9a034b9d77f143d18157d71631305b02?t=344)

![generated-image-at-00:05:44](https://loom.com/i/d79e22a4e3554ed48e63fe3b3b6d547b?workflows_screenshot=true)

- Click 'Yes' to connect to the virtual machine.
- Once connected, you can set up applications like Active Directory.

### Cautionary Notes

- Always save your key pair securely; losing it may prevent access to your virtual machine.
- Log out of your virtual machine when not in use to avoid unnecessary charges on your AWS account.

### Tips for Efficiency

- Familiarize yourself with the AWS interface to speed up the process.
- Keep a record of your key pairs and instance names for easy reference.


---

## Outcome
A Windows EC2 virtual machine was successfully launched and accessed via RDP using a decrypted administrator password, providing a ready server environment for additional lab work.
