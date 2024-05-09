# Project Title: Network Traffic Analysis with Wireshark

## Overview:
This project demonstrates the setup and usage of Wireshark on Ubuntu for capturing and analyzing network traffic. It includes tasks such as installing Wireshark, capturing Ethernet traffic, filtering HTTPS packets, detecting website visits, and applying advanced display filters. The project aims to showcase proficiency in network analysis tools and techniques.

## Tools Used:

-Ubuntu

-Wireshark

## Tasks:

### Task 1: Installation and Setup of Wireshark:

--Use the add-apt-repository command: sudo add-apt-repository ppa:wireshark-dev/stable.

-Install Wireshark using package manager.

-Wireshark should not be run as superuser for security reasons.

-Add the current user to the Wireshark group for packet capture capabilities: sudo usermod -aG wireshark $USER.


### Task 2: Starting Packet Capture on Ethernet Port:

-Demonstrate the ability to capture Ethernet network traffic on the server.

-Identify the wired interface for Ethernet packet capture, typically starting with 'en'.

-Clear browser cache then start packet capture on the Ethernet interface 

-Visit multiple websites, stop scan and save it to a file.


### Task 3: Filtering HTTPS Packets:


-Use a display filter to detect HTTPS packets: tcp.port==443.

-Showcase the detection of certain IP addresses during traffic analysis.

-Utilize conditional statements to include or exclude packets based on IP addresses.


### Task 4: Detecting Website Visits and IP Address:

-Visit a web page (DcukDuckGo and  Google) and detect the IP address using a display filter:


-Use a TLS handshake filter to detect website visits: tls.handshake.type==1

-Identify the IP address of a specific website and filter packets using ip.addr.





### Task 5: Filtering HTTPS Packets Excluding a Certain IP Address:



-Create a filter to display all HTTPS packets while excluding packets from a specific IP address.

-The IP address is used in a filter to obtain packet information for a particular website:
	ip.addr==142.####### 

 Filter packets using src to view all traffic come from the source IP ##### (Google)

Filter packets using src to view traffic that has IP ##### as desination   

Locate all HTTPS packets from a capture not containing a certain IP address:
-A Conditional statement may be used to include and eliminate packets from a Wireshark capture
	- !(ip.addr== 8.43.####) and tcp.port==443)





## Outcome:
This project will result in a comprehensive portfolio piece demonstrating proficiency in network traffic analysis using Wireshark on Ubuntu. It showcases the ability to install, configure, and effectively use Wireshark for capturing and analyzing network packets, making it a valuable asset for networking and cybersecurity roles.








 




