# WiresharkPackageCapture

Task 1
Install and set up Wireshark on Ubuntu:
-Use the add-apt-repository command: 
	-sudo add-apt-repository ppa:wireshark-dev/stable
-Wireshark should not be run as superuser for security reasons.
-The user can be added to the Wireshark group to add packet capture capabilities:
	-sudo usermod-aG wireshark $USER

Task 2
Start a packet capture on an ethernet port and save it to file:
-The wired interface includes the ethernet packet capture, which begins with 'en' in Wireshark.

Task 3 
Use a display filter to detect HTTPS packets:
-To display certain packets in an existing packet capture, use a display filter
-To display only HTTPS traffic, use a filter on TCP port 443: 
	-tcp.port==443

Task 4
Visit a web page and detect it's IP address using a display filter:
-A TLS handshake display filter may be used to detect a website visit in a packet list:
	-tls.handshake.type==1
-The IP address is used in a filter to obtain packet information for a particular website:
	ip.addr==142.####### 

Task 5
Locate all HTTPS packets from a capture not containing a certain IP address:
-A Conditional statement may be used to include and eliminate packets from a Wireshark capture
	- !(ip.addr== 8.43.####) and tcp.port==443)



Misc: 
-Wants to be able to capture ethernet network web traffic on the server and be able to detect certain IP address

-Start a packet capture on an ethernet port and save it to file. 

-Use a display filter to detect HTTPS packets.

Go to web browser, clear cache

Start a capture, visit multiple websites, stop the capture, and eliminate packets from one IP address from the display
