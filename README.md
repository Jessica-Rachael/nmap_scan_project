# nmap_scan_project
I am doing an internship in oasis infobyte under the domain security analysis. So, my first task is to scan localhost and detect open ports using Nmap

Nmap scan project

command used:
nmap -sV 127.0.0.1

purpose:
to scan the local machine for open ports

what is found:
port 135 - msrpc
port 445 - microsoft-ds?
port 8090 - tcpwrapped

significance of each open port:
-port 135 (msrpc):
   Microsoft Remote Procedure Call is used internally by windows for remote management,file sharing and windows service communication

-port 445 (microsoft-ds):
   it is used for server message block which enables file sharing,printer sharing 

-port 8090 (tcpwrapped):
   8090 is a custom port and tcpwrapped means nmap tried to scan the service but it was protected by TCP wrappers or a firewall

screenshot:
screenshots of the nmap terminal output is attached as 'nmap_screenshot.png'.

tools that I have used:
-Nmap for scanning
-windows command prompt

conclusion:
These ports show that some windows networking services are active

This project was done as a part of learning network scanning.
