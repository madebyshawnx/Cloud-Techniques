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
## Setting Up a Two-Tier Architecture in Azure

**1. Introduction to Two-Tier Architecture** [0:02](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=2)
![image alt](

- Overview of the lab's purpose: setting up a two-tier architecture in Azure.
- Explanation of components: 
  - Resource Group: Manages resources.
  - Virtual Network: Contains two subnets for application and database servers.

**2. Logging into Azure** [1:03](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=63)


- Ensure you have an Azure account.
- Log into the Azure portal.

**3. Creating a Resource Group** [1:15](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=75)


- Click on 'Create Resource'.
- Create a new resource group (e.g., RG Lab O3).
- Follow naming conventions.

**4. Creating a Virtual Network** [1:35](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=95)


- Create a virtual network within the resource group.
- Name the virtual network (e.g., The Nets).
- Configure security settings (encryption options).

**5. Creating Subnets** [2:31](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=151)


- Split the virtual network into two subnets: 
  - Web Subnet (e.g., S-net Web).
  - Database Subnet (e.g., S-net DB).
- Assign IP ranges (e.g., /24).

**6. Creating Virtual Machines** [5:27](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=327)


- Navigate to 'Virtual Machines' and click 'Create'.
- Create the first VM (Application Server): 
  - Name it (e.g., VM Web O3).
  - Choose Linux instance (e.g., Ubuntu).
  - Configure SSH key pair.

**7. Configuring VM Settings** [7:23](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=443)


- Set disk type to Standard SSD.
- Select the virtual network and subnet (Web Subnet).
- Enable public IP for the application server.

**8. Creating the Second Virtual Machine** [9:35](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=575)


- Repeat the process to create the second VM (Database Server): 
  - Name it (e.g., VM DB O3).
  - Choose Linux instance.
  - Set it to private (no public IP).

**9. Connecting to the Application Server** [12:18](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=738)


- Connect to the first VM (Application Server) using SSH.

**10. Testing Connectivity to Database Server** [14:20](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=860)


- Use the ping command to test connectivity from the application server to the database server.

**11. Configuring Network Security Group (NSG)** [16:14](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=974)


- Navigate to the NSG settings for the database server.
- Create a new inbound security rule to allow traffic from the application server.

**12. Conclusion** [19:01](https://loom.com/share/63c748cf2a134119882dd8af1c4bd4aa?t=1141)


- Summary of the lab: 
  - Created a resource group, virtual network, and two VMs in separate subnets.
  - Validated connectivity between the application and database servers.


------------------------------------------------------------------------

## Outcome

Successfully deployed a secure two-tier architecture in Azure with
proper network segmentation, controlled access between tiers, and
validated public-to-private traffic flow.
