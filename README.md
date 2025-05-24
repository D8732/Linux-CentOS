#  Description:
This project demonstrates my hands-on setup and configuration of a DNS server using BIND on a Redhat Linux virtual machine. The goal was to build and troubleshoot a fully functional internal DNS system from the ground up.


# Key Features:
Installed and configured the BIND (named) service on CentOS

Set up and validated forward zone files with accurate SOA, NS, and A records

Customized the named.conf file to define authoritative zones and control access

Used systemctl, and other tools to manage and secure the service

Diagnosed and resolved issues such as:

Verified DNS resolution using:

dig

nslookup

named-checkconf and named-checkzone



# Screenshots:
Screenshots of my terminal output, zone file structure, configuration files, and DNS query results will be included to document each step of the process.

Run ifconfig command to see what my ip address is ![ifconfig](https://github.com/user-attachments/assets/60efd6bd-2024-480d-b23e-b4b57d2da9e5)


Before install of the Bind package for dns must check if you have it first the rpm | grep command will check for all files in system associated with bind.

![Checking Bind](https://github.com/user-attachments/assets/16227f5f-5eb9-412d-bd0a-4c03a8319cf3)





Installing bind with dnf command which goes out to the internet to get packages.

![Installing Bind](https://github.com/user-attachments/assets/b8075c16-2d7c-4855-955b-1be6ec97c651)



Used VI command to edit DNS entry were I added the IP address to be used for the DNS server after the 127.0.0.1; 

![Editing Dns configuration](https://github.com/user-attachments/assets/281ecf5d-fa82-4f37-a440-340cefcc7771)


Create zone files with touch command were entries will be held.

![creating files with touch command](https://github.com/user-attachments/assets/7324af17-3796-4dbf-bd72-19eb0d25c1a6)

Used the LS -Ltr command to confirm files were added

![check files that were created ls -ltr](https://github.com/user-attachments/assets/77994f13-8f3e-4b0e-ac82-2b0c30570254)

Used the named-checkzone command to confirm there where no errors with the zones

![check to see if zone is ok](https://github.com/user-attachments/assets/a2a8b502-0401-4948-af27-eecc3cd147a2)



Using systemctl command to start dns service

![Screenshot 2025-05-23 105036](https://github.com/user-attachments/assets/1d1722c3-ad28-44a5-b05e-8c347713efce)

Used VI command to edit Network Manager System commands for enp0s3

![Screenshot 2025-05-23 105934](https://github.com/user-attachments/assets/8a1343f1-014d-4fdf-935c-857a7e299df6)

Add DNS entry

![Screenshot 2025-05-23 110112](https://github.com/user-attachments/assets/ec2bd80d-2ed7-4ab8-aa15-c63859433625)

Use the Nslookup command to resolve the ip address can also use Dig command as well.

![Screenshot 2025-05-23 130155](https://github.com/user-attachments/assets/6d799cec-5f35-436a-b812-8f266e4fc126)

Dig Command does the same as NSlookup, but gives more details.

![image](https://github.com/user-attachments/assets/1531c36d-9924-43dc-93a0-0ad40fe2187b)

# Skills Practiced:
Linux system administration

DNS fundamentals and troubleshooting

Configuration file management

BIND9 and CentOS service setup

