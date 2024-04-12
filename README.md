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
## OUTPUT 
![Screenshot 2024-04-12 195404](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/eb7e295c-dd85-4b14-ac53-810b9c4c9d7a)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT 
![image](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/c0579dcc-0ad4-431e-994a-879df975a785)



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## OUTPUT 
![Screenshot 2024-04-12 195754](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/c1bab2a8-2fbe-4af4-9274-b28b729bbbd7)


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## OUTPUT 
![Screenshot 2024-04-12 195852](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/414c7c46-6fb3-4881-a213-616f88c541dc)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## OUTPUT 
![Screenshot 2024-04-12 195916](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/1d8801ff-7ed7-4339-ab52-9252ebd6b4dc)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## OUTPUT 
![Screenshot 2024-04-12 195943](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/2cf1c771-f160-4ea9-a112-f929577745b8)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## OUTPUT 
![Screenshot 2024-04-12 200005](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/10d33bf0-0db1-471b-925a-750f437efbc2)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![Screenshot 2024-04-12 200107](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/ce5ffe26-8443-42cd-836f-cd6995400214)

![Screenshot 2024-04-12 200130](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/972de985-30b0-4892-bbde-157ea6f03570)





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
## OUTPUT 
![Screenshot 2024-04-12 200208](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/e2cd7ce2-4041-4433-91ec-9471126f7591)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
![Screenshot 2024-04-12 200301](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/5a6f9edd-ffc2-4d7b-9034-cc025c8e8ad3)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![Screenshot 2024-04-12 200336](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/04d59701-fc2c-4897-a37f-96a002935a5c)


select any username in the first column of the above file and check the same
![Screenshot 2024-04-12 200301](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/17f27f5d-8787-4079-a3b2-45104c796a5e)


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
![Screenshot 2024-04-12 200748](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/20584ed4-36ac-4419-8d33-f20e94c7ba02)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT:
![Screenshot 2024-04-12 200929](https://github.com/DEEPAK22003907/Enumeration/assets/119404520/299699c2-c4c8-49a8-b7e6-01929bbb68d6)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

