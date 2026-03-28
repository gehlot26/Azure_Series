# Day-02: Regions, Availability Zones and Iaas/Paas/Saas

## What are Regions ?
- A region is geographical location/area on the globe where any cloud provider has setup their data centers.
- When we create any resource (like a virtual machine) we choose a region, meaning our data physically lives in that location.
- We should always choose a region closer to our users that will lead to low latency. It's like choosing a city to open a warehouse, closer to the customer faster the delivery.

## What are Availability Zones ?
- Within a single region, there are Availability Zones (AZs), these are separate physical data centers inside that region. Each zone has its own power, cooling and networking.
- If one zone goes down due to flood, fire or powercut, the others keep running. This gives our app high availability.

## Iaas, Paas and Saas
These are the 3 service models of cloud computing which defines how much Microsoft (any cloud provider) manages vs how much we manage.

## IaaS - Infrastructure as a Service
- Azure gives us raw hardware like virtual machine, storage, networking.
- We manage the Operating System, software, everything on top.
- Best for developers who want full control.
eg:- Azure Virtual Machines

## PaaS - Platform as a Service
- Azure gives us a ready platform to deploy our app and also manages Operating System, runtime and servers underneath.
- We manage only our application and data.
- Best for developers who wants to deploy code without managing servers.
eg:- Azure SQL Database

## SaaS - Software as a Service
- A fully ready software delivered over the internet for use. We do not manage anything.
- Best for end users, businesses.
eg:- Microsoft 365, Outlook, Teams.


# The Hotel Analogy is the easiest way to remember this.
- IaaS - empty flat (we setup everything)
- PaaS - furnished flat (basics are done)
- SaaS - hotel (everything is handled)