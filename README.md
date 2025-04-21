# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

## AIM:

To use Google for gathering information and perform enumeration of targets

### STEPS:

#### Step 1:

Install kali linux either in partition or virtual box or in live mode

#### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


#### Step 3:
Open terminal and try execute some kali linux commands

### Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

### Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

#### site:
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com




![site](https://github.com/danush564/Enumeration/assets/98585166/4dac5788-4396-4ef9-ac12-ea704c560375)



#### filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com


![file](https://github.com/danush564/Enumeration/assets/98585166/4310e9e7-e978-416a-bd05-3bd021569461)

#### intext:
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![intext](https://github.com/danush564/Enumeration/assets/98585166/2f21ba70-598f-4b28-a2a6-3a841ebe733a)


#### inurl:
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![inurl](https://github.com/danush564/Enumeration/assets/98585166/c7cd1e2d-f85f-418c-a0d7-98df3e171e9b)

#### intitle:
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
![intittle](https://github.com/danush564/Enumeration/assets/98585166/520e8c55-1455-45d5-9d46-c079bbabc227)



#### link:
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![link](https://github.com/danush564/Enumeration/assets/98585166/e70e1c25-b986-497c-a3ab-0c9233edae11)
#### cache:
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![cache](https://github.com/danush564/Enumeration/assets/98585166/7e2867ee-e0dd-445f-a293-0c6b7fb05649)

 
### DNS Enumeration


#### DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
#### OUTPUT:
![dnsrecon](https://github.com/danush564/Enumeration/assets/98585166/ce6de6df-97c6-4b5f-bf92-fb80762b7ee5)

#### dnsenum
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
![dnsenum](https://github.com/danush564/Enumeration/assets/98585166/f0fa6dcb-819e-456d-b24d-f582b48e56e9)


#### smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![meta-smpt](https://github.com/danush564/Enumeration/assets/98585166/9464e9d3-7f83-40cc-a586-930e4e14e73f)

select any username in the first column of the above file and check the same
![smpt-user-enum](https://github.com/danush564/Enumeration/assets/98585166/442f4bf5-6d05-45f6-97d0-c465dcf831b1)


#### Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
#### Output
  
![telnet](https://github.com/danush564/Enumeration/assets/98585166/8d8d7a5f-8748-409a-8e06-d31d8076fd1a)

#### nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


#### OUTPUT:
 

![nmap](https://github.com/danush564/Enumeration/assets/98585166/76fcf01f-f6a3-483f-b4c0-f3d63de8d644)
 

### RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
