# Student-Management-system
OBJECTIVE-:<br>
To design, configure and maintain a secure segmented network infrastructure capable of hosting a multi-tier Student Management System.

<br>GOAL-:
<br> The primary goal of this architecture is to enforce the Principle of Least Privilege (PoLP) and role-based access control at the network layer.In short, to secure the network by ensuring users only get access to what they absolutely need. By locking away the sensitive database from regular everyday traffic, this setup builds a strong, multi-layered security defense—all while keeping the main application running smoothly for everyone.

<br>DETAILED WORKING-:
<br>To mimic a real-world corporate environment, I divided the network into two physical tiers:
<br>The Data Center Tier: A dedicated switch that only hosts the application infrastructure (the Web Server and Database Server).
<br>The Access Tier: A separate switch where end-users (Admins and Students) connect to the network.

<br>By using a 'Router-on-a-Stick' setup and grouping devices into virtual networks (VLANs), I ensured that traffic between users and servers is strictly controlled. Any time a user tries to access a different part of the network, their request is forced through a central router where my security rules decide if it is allowed to pass.

<br>Core Technologies Implemented-:
<br>VLAN Segmentation,Inter-VLAN Routing,Access Control Lists (ACLs ie the security rules to limit or allow the access)

