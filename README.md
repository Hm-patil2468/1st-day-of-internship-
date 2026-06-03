
2/6/2026
 # 1st-day-of-internship-Part 
 
 A:  Information
Host Name : Hp-proDoesk

IPv4 Address.: 192.168.0.1 192.168.1.1

Physical Address (MAC). : 00-1A-2B-3C-4D-5E

Default Gateway .  : 192.168.0.10.121

DNS Servers : 8.8.8.8
                                    8.8.4.4

Part B: Basic Networking Concepts

1. What is an IP Address?
An IP (Internet Protocol) Address is a unique number assigned to a device on a network. It helps devices communicate with each other over the internet or a local network.

3. What is a MAC Address?
A MAC (Media Access Control) Address is a unique hardware identifier assigned to a network card by the manufacturer. It is used to identify devices within a local network.

5. What is a Default Gateway?
A Default Gateway is the router that connects a local network to other networks, including the internet. All internet traffic from a device passes through the gateway.

7. What is DNS?
DNS (Domain Name System) converts website names such as google.com into IP addresses so that computers can locate and connect to websites.

9. Difference Between Public IP and Private IP
a) Public IP
b) Private IP
a) Used on the Internet
b) Used inside local networks
a) Assigned by ISP
b) Assigned by router
a) Globally unique
b) Can be reused in different networks
a) Example: 103.45.67.89
b) Example: 192.168.1.10

Part C: Basic Network Diagram

Internet
               |
               |
        Router / Wi-Fi
      IP: 192.168.1.1
               |
               |
         Your Device
      IP: 192.168.1.10
Commands Used

Find Network Information

ipconfig /all
Find MAC Address Only
getmav

Find Hostname
hostname

Find DNS Information

nslookup google.com


Part D: Network Connectivity Test
Windows Commands

1. Display Network Configuration
Command:


ipconfig
Windows IP Configuration

Ethernet adapter Ethernet:

   IPv4 Address : 192.168.1.10
   Subnet Mask . : 255.255.255.0
   Default Gateway . : 192.168.1.1


2. Test Connectivity
Command:


ping google.com
Pinging google.com [142.250.183.14] with 32 bytes of data:

Reply from 142.250.183.14: bytes=32 time=25ms TTL=118
Reply from 142.250.183.14: bytes=32 time=24ms TTL=118
Reply from 142.250.183.14: bytes=32 time=26ms TTL=118
Reply from 142.250.183.14: bytes=32 time=25ms TTL=118

Ping statistics for 142.250.183.14:
    Packets: Sent = 4, Received = 4, Lost = 0 (0% loss)
3. Trace Route
Command:
tracert google.com

Tracing route to google.com

  1    <1 ms    <1 ms    <1 ms  192.168.1.1
  2    10 ms    11 ms    10 ms  ISP Gateway
  3    18 ms    17 ms    19 ms  Regional Router
  4    25 ms    24 ms    26 ms  google.com

Answers to Questions

1. Was the ping successful?
Answer: Yes, the ping was successful. All 4 packets were sent and received with 0% packet loss.

2. How many hops were shown?
Answer: 4 hops were shown in the traceroute output.

3. What is the purpose of traceroute?
Answer: Traceroute is used to identify the path that data packets take from the source computer to the destination server. It helps diagnose network delays and connectivity issues by showing each router (hop) along the route.