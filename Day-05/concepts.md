# Azure Networking Concepts

When we create resources in Azure (like Virtual Machines, Databases) they need to talk to each other and to the internet. Azure networking is the system that makes this possible securely and in a controlled way.

## Virtual Network (VNet)
- A Virtual Network is our own private, isolated network inside azure and all the resources like VMs and databases live inside a VNet.
- Resources inside the same VNet can talk to each other privately without going through the internet.

## Subnets and CIDR
SUBNETS
- A subnet is a smaller division inside a VNet. We can split our VNet into subnets to organize and separate resources.
- Subnets helps in keeping different types of resources separate and also helps in applying different security rules to different parts.

CIDR
- CIDR is just a way of writing an IP address range using a slash notation.
- eg:- 10.0.0.0/16 where, 
- 10.0.0.0 -> starting IP addresses
- /16      -> no of IPs available in this range
    
- [ smaller the number after / -> more IPs available ]
- [ bigger the number after / -> fewer IPs available ]

## Route
A route is a rule that tells network traffic where to go.

## Route Table
A route table is a collection of routes attached to a subnet.

## Network Security Groups (NSGs)
- A network security group is a firewall that controls what traffic is allowed in and out of a subnet or a virtual machine.
- NSGs can be attached to, 
        . A subnet - applies to all resources inside that subnet
        . single VM - applies only to that VM.

## Application Security Groups (ASGs)
- Application Security Groups are a smarter way to apply NSG rules.
- Instead of using IP addresses, we can group VMs by their role and apply rules to the group.