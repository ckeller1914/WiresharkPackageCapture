# Project Title: Network Traffic Analysis with Wireshark

## Overview:
This project demonstrates the setup and usage of Wireshark on Ubuntu for capturing and analyzing network traffic. It includes tasks such as installing Wireshark, capturing Ethernet traffic, filtering HTTPS packets, detecting website visits, and applying advanced display filters. The project aims to showcase proficiency in network analysis tools and techniques.

## Tools Used:

-Ubuntu

-Wireshark

## Tasks:

### Task 1: Installation and Setup of Wireshark:

-Use the add-apt-repository command to add the Wireshark repository: sudo add-apt-repository ppa:wireshark-dev/stable.

-Install Wireshark using package manager.

-Add the current user to the Wireshark group for packet capture capabilities: sudo usermod -aG wireshark $USER.

-Use the add-apt-repository command: 
	-sudo add-apt-repository ppa:wireshark-dev/stable
-Wireshark should not be run as superuser for security reasons.
-The user can be added to the Wireshark group to add packet capture capabilities:
	-sudo usermod-aG wireshark $USER

### Task 2: Starting Packet Capture on Ethernet Port:

-Demonstrate the ability to capture Ethernet network traffic on the server.

-Identify the wired interface for Ethernet packet capture, typically starting with 'en'.

-Clear browser cache then start packet capture on the Ethernet interface 

-Visit multiple websites, stop scan and save it to a file.

Start a packet capture on an ethernet port and save it to file:
-The wired interface includes the ethernet packet capture, which begins with 'en' in Wireshark.


### Task 3: Filtering HTTPS Packets:

-Apply filters to eliminate packets from specific IP addresses from the display.

-Use a display filter to detect HTTPS packets: tcp.port==443.

-Showcase the detection of certain IP addresses during traffic analysis.

Use a display filter to detect HTTPS packets:
-To display certain packets in an existing packet capture, use a display filter
-To display only HTTPS traffic, use a filter on TCP port 443: 
	-tcp.port==443

### Task 4: Detecting Website Visits and IP Address:


-Use a TLS handshake filter (tls.handshake.type==1) to detect website visits.

-Identify the IP address of a specific website and filter packets using ip.addr.

Visit a web page and detect it's IP address using a display filter:
-A TLS handshake display filter may be used to detect a website visit in a packet list:
	-tls.handshake.type==1
-The IP address is used in a filter to obtain packet information for a particular website:
	ip.addr==142.####### 

### Task 5: Filtering HTTPS Packets Excluding a Certain IP Address:

-Utilize conditional statements to include or exclude packets based on IP addresses.

-Create a filter to display all HTTPS packets while excluding packets from a specific IP address.

Locate all HTTPS packets from a capture not containing a certain IP address:
-A Conditional statement may be used to include and eliminate packets from a Wireshark capture
	- !(ip.addr== 8.43.####) and tcp.port==443)




Filter packets using src to view all traffic come from the source (Google)

Filter packets using src to view traffic that has IP ##### as desination   

Visit DuckDuckGo and Google

Filter for tls handshake

Find client Hello 

Make filter using only packets with IP address #####


Make filter to display all HTTPS traffic along with IP address 


Make filter to display all traffic that is not ip #####

Make filter with a And/or condition






Outcome:
This project will result in a comprehensive portfolio piece demonstrating proficiency in network traffic analysis using Wireshark on Ubuntu. It showcases the ability to install, configure, and effectively use Wireshark for capturing and analyzing network packets, making it a valuable asset for networking and cybersecurity roles.








 




