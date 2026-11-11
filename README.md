Week 2 – Project Module 1: Footprinting & Reconnaissance

Cybersecurity & Ethical Hacking | Kali Linux

Project overview

This project documents a footprinting and reconnaissance lab using six
Kali Linux tools to collect publicly available information about the
assignment’s target domain, networkwalks.com.

The purpose of reconnaissance is to understand a domain’s publicly
visible registration, DNS, web technology, HTTP, and
web-application-firewall information. The work in this lab is for
educational purposes and should only be performed against systems you
are authorized to assess.

Objectives

• Review public domain registration information.
• Identify technologies exposed by the website.
• Resolve the domain name to an IP address.
• Inspect HTTP response headers.
• Check for a web application firewall (WAF).
• Enumerate publicly visible DNS records.
• Save command output and screenshots as evidence.

Tools and commands

Run these commands in a Kali Linux terminal, within the scope of the
assignment:

────────

Task              Tool              Command                              Purpose

────────

1                 WHOIS             whois networkwalks.com             Review public
domain
registration
details and name
servers.

2                 WhatWeb           whatweb networkwalks.com           Identify web
technologies and
server
information
exposed by the
site.

3                 Nslookup          nslookup networkwalks.com          Resolve the
domain name using
DNS.

4                 cURL              curl -I https://networkwalks.com   Retrieve the
website’s HTTP
response headers.

5                 WAFW00F           wafw00f networkwalks.com           Check whether a
web application
firewall is
detected.

6                 DNSRecon          dnsrecon -d networkwalks.com       Enumerate publicly visible DNS records.

Results and observations

Add your own findings from the commands below. Do not copy example
values from the assignment guide as if they were your results; record
what your Kali Linux terminal actually returned.

Task 1 – WHOIS

Purpose: Review the domain’s public registration information.

Findings:
Add a short summary of the registrar, registration/expiry information,
and name servers shown in your output.

Evidence: screenshots/01-whois.png

Task 2 – WhatWeb

Purpose: Fingerprint technologies visible on the website.

Findings:
Summarize the technologies, server details, or other information
reported by WhatWeb.

Evidence: screenshots/02-whatweb.png

Task 3 – Nslookup

Purpose: Resolve the domain name to an IP address.

Findings:
Record the DNS answer and IP address returned by your command.

Evidence: screenshots/03-nslookup.png

Task 4 – cURL

Purpose: Inspect HTTP response headers.

Findings:
Summarize the HTTP status and relevant response headers returned by
your command.

Evidence: screenshots/04-curl-headers.png

Task 5 – WAFW00F

Purpose: Check for a web application firewall.

Findings:
Record whether a WAF was detected and the result reported by the tool.

Evidence: screenshots/05-wafw00f.png

Task 6 – DNSRecon

Purpose: Enumerate publicly visible DNS records.

Findings:
Summarize the DNS record types and relevant results returned by
DNSRecon.

Evidence: screenshots/06-dnsrecon.png

Key learning outcomes

This lab demonstrates how different reconnaissance tools provide
complementary views of a domain:

• WHOIS provides public registration information.
• WhatWeb identifies technologies exposed by a website.
• Nslookup helps resolve domain names through DNS.
• cURL makes it possible to inspect HTTP response headers.
• WAFW00F checks for indications of a web application firewall.
• DNSRecon gathers information about publicly visible DNS records.

Reconnaissance helps security professionals understand an organization’s
external footprint. The same techniques can help defenders identify
information that their own systems expose publicly and decide what
should be protected or reduced.

Repository structure

Organize your repository like this:

Second-week-cybersecurity-project-1/
├── README.md
├── screenshots/
│   ├── 01-whois.png
│   ├── 02-whatweb.png
│   ├── 03-nslookup.png
│   ├── 04-curl-headers.png
│   ├── 05-wafw00f.png
│   └── 06-dnsrecon.png
└── outputs/
    ├── whois.txt
    ├── whatweb.txt
    ├── nslookup.txt
    ├── curl-headers.txt
    ├── wafw00f.txt
    └── dnsrecon.txt

Create the screenshots and outputs folders and add your own evidence
files. If you did not save text outputs, you can omit the outputs
folder.

Conclusion

The project provided practical experience with six Kali Linux
reconnaissance tools and showed how publicly available domain, web,
HTTP, and DNS information can be collected and documented. These
techniques are useful for understanding an organization’s external
attack surface and supporting defensive security assessments.

Disclaimer: Educational use only. Only perform reconnaissance on
domains and systems where you have permission or where the activity is
explicitly authorized.
<img width="1279" height="799" alt="image" src="https://github.com/user-attachments/assets/efeffd63-3c7d-4ccc-b4be-24da0c362558" />
<img width="1282" height="810" alt="image" src="https://github.com/user-attachments/assets/14027976-f8e9-450d-bcc0-c48104554f32" />
<img width="1288" height="804" alt="image" src="https://github.com/user-attachments/assets/6f8175b4-d6c4-42a2-90c0-e68d163fa18b" />
<img width="1281" height="798" alt="image" src="https://github.com/user-attachments/assets/c899ee71-fa61-47c8-98da-66a42abccf19" />
<img width="1282" height="801" alt="image" src="https://github.com/user-attachments/assets/14617be6-b3e6-4222-ab5a-7489205a023f" />
<img width="1282" height="807" alt="image" src="https://github.com/user-attachments/assets/28310282-23b5-48d4-8cea-dd96c9a49f3d" />
