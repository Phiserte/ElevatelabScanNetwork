## Local network recon using NMAP and WIRESHARK

## Objectives

Discover hosts in the local network.
- Identify open ports and services.
- Analyze network scan traffic using Wireshark.
- Document and interpret potential risks.

## Tools Used
- Nmap – for host discovery and port scanning.
- Wireshark– for packet capture and SYN scan verification.
- Linux Terminal– command-line environment.
## Steps 
- Identify the ip address using ifconfig command
- Scan the network with Nmap commad  ''' nmap -sS 192.168.184.0/24''' which sends TCP SYN packets to ip address
- Capture the packets using wireshark with the filter set for tcp packets and specific ip address
## Explnation open ports
- Open ports are network ports which keeps listneing to incoming connections and responds to the connction attempts
- These ports become potential attack surface if there are known vulnarebilities , misconfiguration
- Examples
  3306 - Mysql port can be misconfigured , injection vectors etc
  22 - Ssh port used for remote login exploited becoz of weak keys
  21 - FTP file transfer maybe exploted becoz of directory traversal
  etc 
