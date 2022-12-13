Jose Cardozo
12/13/2022

https://www.varonis.com/blog/port-scanning-techniques
https://www.professormesser.com/network-plus/n10-008/n10-008-video/common-ports-n10-008/

A port scanner is a computer program that checks network ports for one of three possible statuses – open, closed, or filtered.
Port scanners are valuable tools in diagnosing network and connectivity issues. However, attackers use port scanners to detect possible access points for infiltration
and to identify what kinds of devices you are running on the network, like firewalls, proxy servers or VPN servers.
A port scanner sends a network request to connect to a specific TCP or UDP port on a computer and records the response.
So what a port scanner does is send a packet of network data to a port to check the current status. If you wanted to check to see if your web server was operating
correctly, you would check the status of port 80 on that server to make sure it was open and listening.
The status helps network engineers diagnose network issues or application connectivity issues, or helps attackers find possible ports to use for infiltration into
your network.
What is a Port?
A port is a virtual location where networking communication starts and ends (in a nutshell). For a more in-depth explanation, we need to establish a little background
information. There are two kinds of network ports on each computer (65,536 of each for a total of 131,082 network ports):TCP and UDP.
A port scanner sends a TCP or UDP network packet and asks the port about their current status. The three types of responses are below:
Open, Accepted: The computer responds and asks if there is anything it can do for you.
Closed, Not Listening: The computer responds that “This port is currently in use and unavailable at this time.”
Filtered, Dropped, Blocked: The computer doesn’t even bother to respond.
Port scans generally occur early in the cyber kill chain, during reconnaissance and intrusion. Attackers use port scans to detect targets with open and unused ports
that they can repurpose for infiltration, command and control, and data exfiltration or discover what applications run on that computer to exploit a vulnerability in 
that application.
The simplest port scans are ping scans. A ping is an Internet Control Message Protocol (ICMP) echo request – you are looking for any ICMP replies, which indicates 
that the target is alive. A ping scan is an automated blast of many ICMP echo requests to different targets to see who responds. Ping scans aren’t technically port
scanning techniques, as the best you can get back is that there is a computer on the other end, but it’s related and usually the first task before you do a port scan.
One of the more common and popular port scanning techniques is the TCP half-open port scan, sometimes referred to as an SYN scan. It’s a fast and sneaky scan that tries
to find potential open ports on the target computer.
As a network administrator, you will work often with TCP and UDP port numbers, and it’s important to know what some of the most common ports are that you will see 
communicating over your network. The telecommunication network protocol, or what we commonly call Telnet, communicates over TCP port 23. If you need to get a console
screen from a remote device, this allows you to connect to that device remotely, and you’re able to view information on the single terminal screen.
Sometimes you’ll hear this referred to as the console access to that device. But telnet has one significant problem. It sends this information across the network
without any type of encryption. It is sent in the clear from one side of the network to the other.
And because we’re usually logging in with a username and a password, if somebody was able to gather these packets across the network, they’d be able to see all of this
information that we’re transmitting. Because of these security concerns, you don’t commonly see telnet being used for these terminal communications.
Instead, you would use a much more secure protocol such as SSH, or Secure Shell. This communicates over TCP port 22. And although this looks identical to the telnet 
console we were looking at previously, all of this information was sent across the network in encrypted form. If you need to connect to a switch, a router, or firewall,
or any other server on the network using this terminal communication. Then you need to use SSH over TCP port 22.
