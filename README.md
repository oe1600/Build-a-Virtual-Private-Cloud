# Introducing Today's Project!

# Build-a-Virtual-Private-Cloud

# What is Amazon VPC?

Amazon VPC (Virtual Private Cloud) lets users create a secure, isolated
network within AWS. It enables customization of IP ranges, enhances security
with access controls, ensures scalability, and integrates easily with other AWS
services.

# How I used Amazon VPC in this project

I used Amazon VPC to create a secure network in today's project. I set up
public and private subnets, configured route tables, and attached an internet
gateway. This ensured my web servers were secure while providing scalable
internet access.


# One thing I didn't expect in this project was...

One thing I didn't expect in this project was the complexity of configuring
security groups and network ACLs. I underestimated how crucial these settings
are for managing traffic and ensuring proper access, which added more time to
the setup process.

# This project took me...

This project took me about one hour to complete. I quickly set up the Amazon
VPC, configured the necessary subnets and security settings, and deployed
the resources efficient

# Virtual Private Clouds VPCs

A Virtual Private Cloud (VPC) is a private section of a cloud provider's network
where you control your resources, security, and networking. It lets you create
subnets, manage traffic, and securely connect to the internet or other networks
like a VPN

There was already a default VPC in my account ever since my AWS account
was created. AWS provides it to simplify launching resources with preconfigured subnets, internet access, and routing without needing a custom
setup.

To set up my VPC, I had to define an IPv4 CIDR, which means specifying a
block of IP addresses using Classless Inter-Domain Routing. Itʼs written as an IP
followed by a / and a number, determining the size of the address range.

<img src="VPC set up page 1.png" height="80%" width="80%"/>

# Subnets

Subnets are smaller segments of a larger network that help organize and
manage IP addresses within a VPC. They can be public or private, enhancing
security and traffic control while optimizing resource allocation and
accessibility.

There are already subnets in my account, one for every Availability Zone in my
default VPC. These subnets simplify resource deployment by providing a
ready-to-use network setup with public IP access, allowing for quick and
efficient launches

I named my subnet Public 1, but that doesnʼt automatically make it a public
subnet. For a subnet to be public, it must have a route table with a route to an
internet gateway, and instances within it need public IP addresses assigned.

# Internet gateways

Internet gateways are components in a VPC that enable communication
between resources and the Internet. They allow instances in public subnets to
access the internet, providing a target in route tables and enabling network
address translation (NAT).

Attaching an internet gateway to a VPC enables direct communication between
the VPC and the internet. This allows instances in public subnets to access the
internet and receive inbound traffic for hosting applications.
