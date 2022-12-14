Jose Cardozo
12/29/2022

https://www.cyberark.com/what-is/active-directory/

Active Directory
Active Directory (AD) is Microsoft’s directory and identity management service for Windows domain networks. It was introduced in Windows 2000, is included with most MS Windows Server operating systems, and is used by a variety of Microsoft solutions like Exchange Server and SharePoint Server, as well as third-party applications and services.

AD is made up of a number of different directory services, including:
Active Directory Domain Services (AD DS) – the core Active Directory service used to manage users and resources.
Active Directory Lightweight Directory Services (AD LDS) – a low-overhead version of AD DS for directory-enabled applications.
Active Directory Certificate Services (AD CS) – for issuing and managing digital security certificates.
Active Directory Federation Services (AD FS) – for sharing identity and access management information across organizations and enterprises.
Active Directory Rights Management Services (AD RMS) – for information rights management (controlling access permissions to documents, workbooks, presentations, etc.)

Fundamental AD features and capabilities include:
A schema that defines the classes of objects and attributes contained in the directory.
A global catalog that contains detailed information about every object in the directory.
A query and index mechanism that allows users, administrators, and applications to efficiently find directory information.
A replication service that disseminates directory data across the network.

AD Domain Services Overview
Active Directory Domain Services is the primary Active Directory service. It is used to authenticate users and to control access to network resources. A server running AD DS is called a domain controller. Most Windows domain networks have two or more domain controllers; a primary domain controller and one or more backup domain controllers for resiliency. During login, users authenticate to a domain controller and are granted access to particular resources based on administratively defined policies.

AD Data Structures
Active Directory stores information about network users (names, phone numbers, passwords, etc.) and resources (servers, storage volumes, printers, etc.) in a hierarchical structure consisting of domains, trees, and forests.

A domain is a collection of objects (e.g. users, devices) that share the same Active Directory database. A domain is identified by a DNS name like company.com.
A tree is a collection of one or more domains with a contiguous namespace (they have a common DNS root name like marketing.company.com, engineering.company.com, and sales.company.com).
A forest is a collection of one or more trees that share a common schema, global catalog, and directory configuration—but aren’t part of a contiguous namespace. The forest typically serves as the security boundary for an enterprise network.

AD Benefits
Active Directory provides a variety of functional and business benefits, including:

Security – Active Directory helps businesses improve security by controlling access to network resources.
Extensibility – companies can easily organize Active Directory data to align with their organizational structure and business needs.
Simplicity – administrators can centrally manage user identities and access privileges across the enterprise, helping businesses simplify management and reduce operations expenses.
Resiliency – Active Directory supports redundant components and data replication to enable high availability and business continuity.
