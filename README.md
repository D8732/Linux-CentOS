#  Description:
This project demonstrates my hands-on setup and configuration of a DNS server using BIND on a CentOS Linux virtual machine. The goal was to build and troubleshoot a fully functional internal DNS system from the ground up.


Key Features:
Installed and configured the BIND (named) service on CentOS

Set up and validated forward zone files with accurate SOA, NS, and A records

Customized the named.conf file to define authoritative zones and control access

Used systemctl, firewalld, and SELinux tools to manage and secure the service

Diagnosed and resolved issues such as:

“bad owner name” errors

failed zone loads

named service startup failures

Verified DNS resolution using:

dig

nslookup

named-checkconf and named-checkzone



# Screenshots:
Screenshots of my terminal output, zone file structure, configuration files, and DNS query results will be included to document each step of the process.

Run ifconfig command to see what my ip address is "C:\Users\USER\OneDrive\Pictures\Screenshots\ifconfig.png"










# Skills Practiced:
Linux system administration

DNS fundamentals and troubleshooting

Configuration file management

BIND9 and CentOS service setup

