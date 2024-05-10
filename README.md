# Project Title: Network Traffic Analysis with Wireshark

## Overview:
This project demonstrates the setup and usage of Wireshark on Ubuntu for capturing and analyzing network traffic. It includes tasks such as installing Wireshark, capturing Ethernet traffic, filtering HTTPS packets, detecting website visits, and applying advanced display filters. The project aims to showcase proficiency in network analysis tools and techniques.

## Tools Used:

-Ubuntu

-Wireshark

## Tasks:

### Task 1: Installation and Setup of Wireshark:

	1a) Install Wireshark on a virtual machine using Ubuntu

![DL Wireshark](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/09db9ccd-a764-4c6a-9078-f33f5a626244)


	1b) Wireshark should not be run as superuser for security reasons.

	1c) Add the current user to the Wireshark group for packet capture capabilities: *sudo usermod -aG wireshark $USER*.

![SudoMod](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/36cd462c-c71f-4908-92ce-8be1fc787fe7)


### Task 2: Starting Packet Capture on Ethernet Port:

	2a) Clear cache in user's browser settings. 

![ClearCache](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/50cfad92-e0de-446c-ae7f-2ccb2e7a00cd)

	2b) After installation pull up Wireshark to run a packet scan.

![startscan](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/87e81fb2-946e-446c-8b99-d71a698174f0)


	2c) Start scan then monitor the network traffic.

![PackCapt1](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/d9979495-bf8c-4159-8ad7-8762bf7d0183)



	2d) After visiting multiple websites, stop scan and analyze packet captures

![443](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/7737c802-18c4-415c-8f4e-b61226b09f9c)


	2e) Save packet captures to a file.

![Save1](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/be816869-73a2-4dfb-b340-c806d4d41ed4)


### Task 3: Filtering HTTPS Packets:


	3a) Use a display filter to detect HTTPS packets: *tcp.port==443*.

![443](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/8388b654-fb91-4364-8700-642e19097112)


	3b) Showcase the detection of certain IP addresses during traffic analysis.

![Screenshot (32)](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/e5bea145-f68c-4a56-89f6-50e99b580fbe)



### Task 4: Detecting Website Visits and IP Address:

	4a) Visit a web page (DcukDuckGo and  Google) and detect the IP address using a display filter:

	4b) Utilize conditional statements to include or exclude packets based on IP addresses.

	4c) Use a TLS handshake filter to detect website visits: 
 
 		-tls.handshake.type==1

![Handshake1](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/1a9f85df-ccd9-4f30-ae7b-5aeb6dabe6dc)


	4d) Identify the IP address of a specific website and filter packets using addr:
 
 		-ip.addr==142.251.16.104

![IP ADR](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/5774d63c-510e-4448-8a86-6d6e8b86cb78)


	4e) Identify the IP source of a specific website and filter packets using  
 
 		-ip.scr==142.251.16.104

![IP SCR](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/1ff67b92-2eec-491f-bbf1-d757286f2248)


	4f) Identify the IP destination of a specific website and filter packets using 
 
 		-ip.dst==142.251.16.104

![IP DST](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/fb826ba1-1076-4c77-ba46-13292a316744)

	4g) Tailor statements to filter multiple conditional: (This filters specific address or anything using HTTPS)
 
 		-ip.addr==142.251.16.104 or tcp.port==443 

![IP Or](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/e0d8064f-4c50-43d3-baa8-361c86bb40fc)



### Task 5: Filtering HTTPS Packets Excluding a Certain IP Address:



	5a) Create a filter to display all HTTPS packets while excluding packets from a specific IP address. 
 
 		!(ip.addr==142.251.16.104) or tcp.port==443

*![Not IP or](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/2d5408f8-b0d7-4e9a-b849-220c24bb33db)*


	5b) Create a filter to exclude all HTTPS packets and packets from a specific IP address. 
 
 		!(ip.addr==142.251.16.104) or (tcp.port==443)
	- 

![Screenshot (50)](https://github.com/ckeller1914/WiresharkPackageCapture/assets/116524804/e96fe3dc-dad3-46c1-bc28-49603bf73bb0)




## Outcome:
This project will result in a comprehensive portfolio piece demonstrating proficiency in network traffic analysis using Wireshark on Ubuntu. It showcases the ability to install, configure, and effectively use Wireshark for capturing and analyzing network packets, making it a valuable asset for networking and cybersecurity roles.








 




