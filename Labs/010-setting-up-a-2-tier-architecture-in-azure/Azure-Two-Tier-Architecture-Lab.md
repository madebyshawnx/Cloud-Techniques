# Azure Two-Tier Architecture Lab

This lab demonstrates how to design and deploy a basic two-tier
architecture in Microsoft Azure using separate web and database virtual
machines.

## Watch me build this lab

https://www.loom.com/share/63c748cf2a134119882dd8af1c4bd4aa

**What this video shows:** Building a secure two-tier architecture in
Azure with separate subnets, virtual machines, and controlled network
access between web and database tiers.

------------------------------------------------------------------------

## Objective

To deploy and configure a basic two-tier architecture in Azure that
separates a web server from a backend database server using proper
networking and security controls.

------------------------------------------------------------------------

## Skills Practiced

-   Designing cloud network architecture
-   Creating and configuring Virtual Networks (VNets)
-   Subnet segmentation and IP address planning
-   Deploying Azure Virtual Machines
-   Configuring Network Security Groups (NSGs)
-   Securing inter-tier communication
-   Validating connectivity between tiers
-   Understanding public vs private access design

------------------------------------------------------------------------

## Tools Used

-   Microsoft Azure Portal
-   Azure Virtual Network (VNet)
-   Azure Virtual Machines
-   Network Security Groups (NSGs)
-   Public IP Address
-   Remote access tools (RDP or SSH)

------------------------------------------------------------------------

## Steps Performed

1.  **Created Resource Group**\
    Created a dedicated Azure Resource Group to logically organize all
    infrastructure components for the lab.\
    (Optional screenshot) docs/step-1.png

2.  **Configured Virtual Network**\
    Defined a Virtual Network (VNet) with an address space to serve as
    the private network boundary for both tiers.\
    (Optional screenshot) docs/step-2.png

3.  **Created Web and Database Subnets**\
    Segmented the VNet into separate subnets for the web server and
    database server to isolate traffic between tiers.\
    (Optional screenshot) docs/step-3.png

4.  **Deployed Web Server Virtual Machine**\
    Provisioned a virtual machine in the web subnet and configured it to
    accept public web traffic (example: ports 80/443).\
    (Optional screenshot) docs/step-4.png

5.  **Configured Web Server Access Rules**\
    Applied Network Security Group rules to allow HTTP/HTTPS traffic
    publicly while restricting administrative access.\
    (Optional screenshot) docs/step-5.png

6.  **Deployed Database Server Virtual Machine**\
    Provisioned a backend virtual machine in the database subnet with no
    public exposure.\
    (Optional screenshot) docs/step-6.png

7.  **Restricted Database Access**\
    Configured Network Security Group rules to allow database traffic
    (example: port 1433) only from the web subnet.\
    (Optional screenshot) docs/step-7.png

8.  **Validated Inter-Tier Connectivity**\
    Tested communication between the web server and database server to
    confirm proper internal routing and security controls.\
    (Optional screenshot) docs/step-8.png

9.  **Verified Public Web Access**\
    Confirmed that the web server was reachable via its public IP
    address while the database server remained private.\
    (Optional screenshot) docs/step-9.png

10. **Reviewed Architecture and Security Design**\
    Reviewed the overall design to ensure proper tier separation,
    minimal public exposure, and controlled traffic flow.\
    (Optional screenshot) docs/step-10.png

------------------------------------------------------------------------

## Outcome

Successfully deployed a secure two-tier architecture in Azure with
proper network segmentation, controlled access between tiers, and
validated public-to-private traffic flow.
