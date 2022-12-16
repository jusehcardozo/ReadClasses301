Jose Cardozo
12/16/2022

https://www.fortinet.com/fr/resources/cyberglossary/what-is-site-to-site-vpn


Site-to-Site VPN Defined

A site-to-site virtual private network (VPN) refers to a connection set up between multiple networks. This could be a corporate network where multiple offices work in conjunction with each other or a branch office network with a central office and multiple branch locations. 

Site-to-site VPNs are useful for companies that prioritize private, protected traffic and are particularly helpful for organizations with more than one office spread out over large geographical locations. These businesses often have to access resources housed on a primary network, which could include servers that facilitate email or store data. In some instances, a server may be the operational hub of an application essential to the company’s business. A site-to-site VPN can, in that case, give all sites full access to the application—as if it were housed within their physical facility.

There are a few different types of SSL VPNs, and each comes with its own benefits. Depending on the needs of your organization, one type may better fit your objectives than others.

Remote Access VPNs
A remote access VPN refers to a temporary connection set up between two or more users and a central location. In most cases, a remote access VPN is used to give each location access to a data center. In some situations, a connection that makes use of Internet Protocol security (IPsec) is sufficient. However, it is also common for an organization to utilize a VPN, which avails them of the security positioned at the gateways at each end of the VPN.

A remote access VPN is a useful tool for companies with remote workers either on the road or in their homes. If these workers need to access private or sensitive information housed in the company’s servers, they can connect to a remote access VPN. In this way, each employee is able to gain access to the resources they need to do their jobs.

Intranet-based Site-to-Site
An intranet-based site-to-site VPN connects more than one local-area network (LAN) to form a wide-area network (WAN). A company may also use this kind of setup to incorporate software-defined WAN (SD-WAN). Intranet-based site-to-site VPNs are useful tools for combining resources housed in disparate offices securely, as if they were all in the same physical location.

An intranet-based site-to-site VPN is particularly helpful if each site either develops its own resources or houses unique processes that the entire company would benefit from having access to. For example, if each office had design schematics that were constantly being updated and adjusted for clients, an intranet-based site-to-site VPN would give decision-makers in a number of offices secure access to everything produced—regardless of their physical location.

Extranet-based Site-to-Site
Extranet-based site-to-site VPNs are often used by two or more different companies that want to share certain resources but keep others private. With an extranet-based site-to-site VPN, each entity connects to the VPN and chooses what they want to make available to the other companies. In this way, they can collaborate and share without exposing proprietary data.

How to Create a Site-to-Site VPN
Creating a site-to-site VPN involves determining how you want the data to be transferred from one site to the next and choosing a way to make sure it is secure from intruders. This can be done with an internet-based site-to-site VPN or a multiprotocol label switching (MPLS) site-to-site VPN.

Creating an Internet-based Site-to-Site VPN
An internet-based site-to-site VPN uses the existing network of an organization in combination with the public internet. To set up an internet-based site-to-site VPN, you need a VPN gateway that secures the data traveling back and forth.

To create an internet-based site-to-site VPN, you make a tunnel that connects two networks, for which you need three components:

A base network in one location
A satellite network in another location
A tunnel with security gateways on each end
The tunnel “burrows through” or sits on top of a physical internet connection. However, the tunnel protects the traffic flowing through it from being accessed by people using the physical network. To set it up, you need to set up a gateway at each site. The first gateway the data meets as it enters the tunnel will encrypt the data. The encryption keeps each data packet safe from users, devices, and malware that could seek to corrupt, steal, or compromise it in some way. 

As the data arrives at its destination, it meets the other gateway. This decrypts the data so the network on the other side can read it. Entities in the physical internet the data has to travel through while encrypted will not be able to read it. The data will remain unreadable without a second gateway to decrypt it for the receiving network.

Creating an MPLS Site-to-Site VPN
MPLS can be a useful tool for organizations wanting to send data between two locations. An MPLS site-to-site VPN depends on infrastructure made available by the VPN provider, as opposed to the company that uses the VPN. The configuration of an MPLS VPN involves creating VPN connections between the primary site and the satellite sites.

Why Implement a Site-to-Site VPN
There are several factors to consider when figuring out whether to implement site-to-site VPN services. In some cases, typical IPsec is sufficient for communication between two or more locations. However, there are a few considerations that may drive a company to use VPN connections instead:

The number of locations
Business size
The distance between each location
The resources the locations have to share with each other
In most cases, a site-to-site VPN is a good solution if your business consists of several locations, each with employees that need to share resources provided by the main office. If you use a site-to-site VPN in this kind of situation, you can ensure that all employees have secure access to the same resources.

5 Key Components of a Site-to-Site VPN
Watertight Security
The VPN your company chooses must be protected by stringent security measures. The data that travels back and forth must be secure, both as it moves from point to point and while at rest in each location. This involves adequate authorization, authentication, and administration. It is also important for all practices to support the security policies of the organization, including any established best practices that have been developed by the various IT staff in each location.

Ease of Operations
If a VPN is difficult to use, it can cause more frustration than convenience. Users should have the freedom to access the VPN using a web browser. While it is important to ensure ease of access, this should not result in lax security practices. If users have to take an extra step to get into the VPN, the extra security may be worth the additional few moments it takes to gain entry.

Simple and Secure Scalability
It is easy to scale a VPN. You can add a new site, user, office, or partner organization in minutes. If you do not have to put additional VPN clients at each new location, it is quick and inexpensive to incorporate additional connections. Also, in case you need to relocate a satellite office, it is easy to set up another location.

Business Continuity
In the event of a disaster, whether naturally caused or due to an infrastructural issue, it is important to minimize business interruption and get back up and running as soon as possible. A site-to-site VPN lets you leverage remote access immediately after an emergency has been identified. 

Flexible Deployment
With a VPN, you have the power to deploy a new solution across a broad network of devices at various physical locations. You can choose which sites to provide the new solution to first, second, and so forth. This could give you the flexibility to offer training or support in controllable phases instead of tackling it all at once and potentially overwhelming your IT team.

