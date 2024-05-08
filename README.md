# WiresharkPackageCapture

Project Title: Network Traffic Analysis with Wireshark on Ubuntu

Overview:
This project demonstrates the setup and usage of Wireshark on Ubuntu for capturing and analyzing network traffic. It includes tasks such as installing Wireshark, capturing Ethernet traffic, filtering HTTPS packets, detecting website visits, and applying advanced display filters. The project aims to showcase proficiency in network analysis tools and techniques.

Tasks:

Task 1: Installation and Setup of Wireshark:

Use the add-apt-repository command to add the Wireshark repository: sudo add-apt-repository ppa:wireshark-dev/stable.
Install Wireshark using package manager.
Add the current user to the Wireshark group for packet capture capabilities: sudo usermod -aG wireshark $USER.
Task 2: Starting Packet Capture on Ethernet Port:

Identify the wired interface for Ethernet packet capture, typically starting with 'en'.
Start packet capture on the Ethernet interface and save it to a file.
Task 3: Filtering HTTPS Packets:

Use a display filter to detect HTTPS packets: tcp.port==443.
Task 4: Detecting Website Visits and IP Address:

Use a TLS handshake filter (tls.handshake.type==1) to detect website visits.
Identify the IP address of a specific website and filter packets using ip.addr.
Task 5: Filtering HTTPS Packets Excluding a Certain IP Address:

Utilize conditional statements to include or exclude packets based on IP addresses.
Create a filter to display all HTTPS packets while excluding packets from a specific IP address.
Miscellaneous:

Demonstrate the ability to capture Ethernet network traffic on the server.
Showcase the detection of certain IP addresses during traffic analysis.
Clear browser cache, start a capture, visit multiple websites, and apply filters to eliminate packets from specific IP addresses from the display.
Additional Features (Not in Tasks):

Video demonstration showcasing the usage of Wireshark filters, including filtering packets using source and destination IP addresses.
Visit specific websites like DuckDuckGo and Google to demonstrate packet analysis.
Use advanced filters to find specific elements like TLS handshake and client hello messages.
Combine filters using logical AND/OR conditions for complex traffic analysis scenarios.
Outcome:
This project will result in a comprehensive portfolio piece demonstrating proficiency in network traffic analysis using Wireshark on Ubuntu. It showcases the ability to install, configure, and effectively use Wireshark for capturing and analyzing network packets, making it a valuable asset for networking and cybersecurity roles.
