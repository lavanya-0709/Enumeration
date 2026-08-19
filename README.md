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
<img width="1919" height="1010" alt="image" src="https://github.com/user-attachments/assets/6824c277-2b76-4067-8330-1ae7df43d3fa" />



filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
<img width="1919" height="1025" alt="image" src="https://github.com/user-attachments/assets/52d86669-dfac-4cb9-a2ee-e5ec6274e309" />




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1919" height="965" alt="image" src="https://github.com/user-attachments/assets/0ba5fbce-4dca-4946-90c5-3978e75019c4" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1917" height="955" alt="image" src="https://github.com/user-attachments/assets/8aa7ed42-fbb4-461c-a2bd-45f784eb2c5e" />


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1919" height="966" alt="image" src="https://github.com/user-attachments/assets/226a6987-d09a-41f2-a29b-4133306312e2" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1917" height="965" alt="image" src="https://github.com/user-attachments/assets/129ccd94-7367-4568-8880-22755178ae9e" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

<img width="900" height="547" alt="Screenshot 2026-08-19 141740" src="https://github.com/user-attachments/assets/373cdd9a-2f6e-41bc-a600-96ff34dfe759" />


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

<img width="919" height="893" alt="Screenshot 2026-08-19 142019" src="https://github.com/user-attachments/assets/078bea09-f703-4653-8784-6394e727bd86" />


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

## OUTPUT
<img width="823" height="506" alt="Screenshot 2026-08-19 142215" src="https://github.com/user-attachments/assets/31e9cf99-f65f-42f3-9666-87c14bef1f01" />


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output
<img width="607" height="168" alt="Screenshot 2026-08-19 142258" src="https://github.com/user-attachments/assets/69b134df-5e31-417d-9694-58d484bea6a6" />
 

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

<img width="757" height="254" alt="Screenshot 2026-08-19 142332" src="https://github.com/user-attachments/assets/4f6ddbb4-27ac-4a57-9419-b30cf8ea5e72" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
