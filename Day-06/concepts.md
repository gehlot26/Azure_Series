# Azure Networking Concepts

## Azure Application Gateway
- Azure Application Gateway is a load balancer for web traffic (HTTP/HTTPS). It sits in front of the web apps and smartly distributes incoming requests.
- It does not balance traffic but also can route traffic to different backends based on the URL.
Eg:- /images -> Server A | /videos -> Server B


## WAF - Web Application Firewall
WAF is a security feature built into App Gateway which protects the web app from common attacks like SQL Injection, Cross Site Scripting and DDoS.


## Azure Load Balancer
- Azure Load Balancer distributes incoming network traffic across multiple VMs so no single VM gets overwhelmed.
- If one VM goes down, load balancer automatically stops sending traffic to it.


## Azure DNS
- Azure Domain Name System is like a phonebook of the internet.
- when we type google.com in the browser, DNS converts it to an IP address like 142.250.80.46 because computers talk in IPs and not names.


## Azure Firewall
- Azure Firewall is a cloud based security service that controls what traffic is allowed in and out of the Azure network.
- It sits at the network level and filters all traffic. we can write rules to allow or block traffic.
- It works across the entire azure network and not just one app.


## VNet Peering
- VNet peering connects two VNets together so resources in both can communicate privately without going through the internet.
- We can also peer VNets in different regions and it will be termed as Global VNet Peering.


## VNet Gateway
A VNet Gateway is used when we want to connect two VNets in more complex setup with routing and encryption.
Eg:- connecting on-premise office network to azure VNet.


## VPN Gateway
VPN Gateway is a specific type of VNet Gateway that creates an encrypted tunnel between on premise network and azure vnet.


## VNet Gateway is the umbrella term. VPN Gateway is one type of it. When we create a VNet Gateway in Azure, it asks to pick a type VPN or ExpressRoute.
## So a VPN Gateway is literally just a VNet Gateway with the type set to 'VPN'.

