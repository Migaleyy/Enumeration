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
Following searches for all the sites that is in the domain yahoo.com

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/356b7f6e-ef9b-454e-91cb-bc1e7ed5d87f)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/1abcc983-f768-4dba-9261-cd526f4abff4)

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/a54fb6ba-5e44-4b50-9a12-84da01f12734)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/7ed16f1c-9db2-430f-8396-bdc3d3ccc886)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/6705efcc-f372-4a63-a689-ec99af3c539b)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/855b3e86-3dd8-4778-8ea5-96ba30013fc9)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/969c021c-6de0-4055-aac2-ddbb98a781cd)

##DNS Enumeration
DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/0a2fe42a-89c5-4df9-8935-099d42b03cae)

![image](https://github.com/Migaleyy/Enumeration/assets/118262199/5bb35d3f-7003-42c5-885a-85370b9d5f85)






##dnsenum
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

##OUTPUT:
![image](https://github.com/Migaleyy/Enumeration/assets/118262199/4f232685-b8a4-4d72-9bda-456b75f3af2f)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/Migaleyy/Enumeration/assets/118262199/84e18785-c368-4586-9b9c-cdebe448a943)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
select any username in the first column of the above file and check the same

![image](https://github.com/Migaleyy/Enumeration/assets/118262199/8198679a-1cd5-43a0-9fd5-ca93d0a7df19)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

![image](https://github.com/Migaleyy/Enumeration/assets/118262199/9605f734-222d-4340-89ea-8cd97a83fa69)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

![image](https://github.com/Migaleyy/Enumeration/assets/118262199/c4ed2e80-7acd-44e4-a45d-020ffec8075f)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

