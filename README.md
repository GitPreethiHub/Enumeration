# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:
To use Google for gathering information and perform enumeration of targets

## STEPS:
### Step 1:
Install kali linux either in partition or virtual box or in live mode

### Step 2:
Investigate on the various Google hacking keywords and enumeration tools as follows:

### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  
Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain linkedin.com

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/4335212a-f31f-43c2-b366-793a8879b7ec)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain linkedin.com

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/e172de10-0e04-4bb5-8d73-a97d501a9b39)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/cb2c427b-7f3f-45ca-8e5c-0681f9f348ad)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/f65aba0e-80f8-4e44-9556-12e4132e4666)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/8318f883-acdd-4fd9-894b-8e4ac4eaa944)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/a48a22ab-16d6-4383-b0d7-504217cd5fe9)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 ![image](https://github.com/Yamunaasri/Enumeration/assets/115707860/ad91e2fa-8fc0-4b65-9219-ae8eea0697ad)

## DNS Enumeration:

## DNS Recon:
Provides the ability to perform:
   Check all NS records for zone transfers
   Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
   Perform common SRV Record Enumeration
   Top level domain expansion

![image](https://github.com/user-attachments/assets/4561c859-3cc6-42e0-a7b3-064c63b80f3d)

![image](https://github.com/user-attachments/assets/3b884c71-c1e9-467f-b3cf-4b471597431c)


## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![image](https://github.com/user-attachments/assets/b658cc77-34cb-4e36-a4f1-e12b09c7fa98)

![image](https://github.com/user-attachments/assets/9104f235-9fef-4563-99ec-86ed498dae6f)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/user-attachments/assets/a2cf3e7c-b4f9-48c0-b238-e039ad52b015)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/user-attachments/assets/4b08f146-dbeb-4fef-8a60-9229d216f14d)

select any username in the first column of the above file and check the same

![image](https://github.com/user-attachments/assets/2a024227-a1b6-4843-b50d-28d85b6e0eb1)

## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

![image](https://github.com/user-attachments/assets/cc3b3048-82b9-49fc-8978-c64dcb6bd6d1)

## nmap –script smtp-enum-users.nse <hostname>
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands.
The goal of this script is to discover all the user accounts in the remote system
![image](https://github.com/user-attachments/assets/bac02036-4f9e-4422-b0a0-3ddf24737a32)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

