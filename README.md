# Enumeration
Enumeration Techniques

### NAME: ESWANTH KUMAR K
### REG NO: 212223040046

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

## Output:
![Screenshot 2024-09-24 211602](https://github.com/user-attachments/assets/8efaaff8-0c53-4fc6-96b2-ec0eda36accd)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output:
![Screenshot (201)](https://github.com/user-attachments/assets/694649fc-0f99-4665-9e9a-87adf894426d)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output:
![Screenshot 2024-09-24 211907](https://github.com/user-attachments/assets/f172fa9d-4301-498b-8927-a1a300a99086)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Output:
![Screenshot (202)](https://github.com/user-attachments/assets/8a161297-0259-498e-81c0-ab2ba209bd35)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output:
![Screenshot 2024-09-24 212249](https://github.com/user-attachments/assets/18160d03-8acb-41a7-892c-1714c9ba0d95)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output:
![Screenshot 2024-09-24 212434](https://github.com/user-attachments/assets/5dd2d822-5dc3-4ea2-9d02-b9225f83c44a)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## Output:
![Screenshot 2024-09-24 214920](https://github.com/user-attachments/assets/e45def3d-98c7-47aa-be0e-027d2bf71226)

# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![Screenshot (203)](https://github.com/user-attachments/assets/035b6a2f-1be8-49c0-b08c-c8e713a4f858)

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
## OUTPUT:
![Screenshot 2024-09-24 220552](https://github.com/user-attachments/assets/acede183-5e92-43aa-8106-8eb2e325ea25)
![Screenshot 2024-09-24 220650](https://github.com/user-attachments/assets/b6f0b741-eea9-4b57-98f3-c860ea5f0a24)
![Screenshot 2024-09-24 220723](https://github.com/user-attachments/assets/45147455-b499-491e-b1a6-c997441a3af5)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## OUTPUT:
![Screenshot 2024-09-24 221508](https://github.com/user-attachments/assets/45316a52-0042-4475-98a5-137249bf2b22)

# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output:
 ![Screenshot (214)](https://github.com/user-attachments/assets/e9a1a401-642a-4675-b790-133db73f36e5)

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![Screenshot (210)](https://github.com/user-attachments/assets/b7ba7244-e8e7-4fcf-ae3f-cfd94f9ad982)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

