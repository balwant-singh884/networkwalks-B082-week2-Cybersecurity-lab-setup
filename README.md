<div align="center">

# 🔐 NetworkWalks Cybersecurity Internship

## Week 02 — Footprinting & Reconnaissance

### W2-PM1: Information Gathering Using Multiple Kali Linux Tools

![Kali Linux](https://img.shields.io/badge/Kali-Linux-blue)
![VMware](https://img.shields.io/badge/VMware-Workstation-orange)
![Batch](https://img.shields.io/badge/Batch-B082-green)
![Reconnaissance](https://img.shields.io/badge/Phase-Footprinting-success)

<br>

Building practical reconnaissance skills through ethical and authorized information gathering using Kali Linux.

</div>

---

# 📌 Project Overview

As part of **Week 02** of the **NetworkWalks Cybersecurity Internship (Batch B082)**, I performed authorized footprinting and reconnaissance activities against the approved target domain:

```text
networkwalks.com
```

The purpose of this exercise was to understand how publicly available information can be collected using different reconnaissance tools and how each tool provides a different perspective on a target's infrastructure.

The activities focused on:

- Domain intelligence gathering
- DNS enumeration
- Website technology identification
- Web Application Firewall detection
- HTTP response analysis
- Documentation and reporting

---

# 🎯 Learning Objectives

- Understand footprinting and reconnaissance concepts
- Gather information from publicly available sources
- Perform DNS enumeration
- Identify website technologies
- Detect Web Application Firewall protections
- Analyze HTTP response headers
- Document findings professionally
- Practice ethical reconnaissance methodologies

---

# 📜 Authorization & Scope

This activity was conducted as part of the **NetworkWalks Cybersecurity Internship Program (Batch B082)**.

Reconnaissance activities were performed only against authorized targets provided within the internship scope.

### Allowed Activities

✅ WHOIS

✅ NSLOOKUP

✅cURL

✅ WhatWeb

✅ Wafw00f



### Prohibited Activities

❌ Exploitation

❌ Denial of Service

❌ Brute Force Attacks

❌ Unauthorized Access Attempts

❌ Privilege Escalation

---

# 📄 Authorization Evidence

### Authorization Letter

📸 **ADD AUTHORIZATION LETTER SCREENSHOT – PAGE 1**

```text
authorization/authorization-page1.png
```

📸 **ADD AUTHORIZATION LETTER SCREENSHOT – PAGE 2**

```text
authorization/authorization-page2.png
```

---

# 🖥️ Lab Environment

| Component | Configuration |
|------------|--------------|
| Host System | Windows 11 |
| Processor | Intel Core i5-12500H |
| Memory | 16 GB RAM |
| Storage | 512 GB SSD |
| Graphics | NVIDIA RTX 3050 |
| Virtualization Platform | VMware Workstation |
| Guest Operating System | Kali Linux |
| Activity Type | Footprinting & Reconnaissance |
| Target Domain | networkwalks.com |

---

# 🛠️ Tools Used

| Tool | Purpose |
|--------|---------|
| WHOIS | Domain registration information |
| NSLOOKUP | DNS resolution |
| cURL | HTTP response header analysis |
| WhatWeb | Website technology identification |
| Wafw00f | Web Application Firewall detection |


---

# 📂 Repository Structure

```text
networkwalks-B082-week2-footprinting-reconnaissance
│
├── README.md
│
├── authorization
│   ├── authorization-page1.png
│   └── authorization-page2.png
│
├── screenshots
    ├── 01-whois.png
    ├── 02-nslookup.png
    ├── 03-curl.png
    ├── 04-whatweb.png
    ├── 05-wafw00f.png

```

---

# 🔎 Reconnaissance Workflow

```text
Target Domain
      │
      ▼
    WHOIS
      │
      ▼
   NSLOOKUP
      │
      ▼
     CURL 
      │
      ▼
   WHATWEB
      │
      ▼
   WAFW00F
      │
      ▼
 Documentation
```

---

# 1️⃣ WHOIS Analysis

## Purpose

WHOIS is used to retrieve publicly available domain registration information.

### Command

```bash
whois networkwalks.com
```

### Evidence

📸 <img width="1563" height="591" alt="whois" src="https://github.com/user-attachments/assets/b01cff2a-e6cb-4a73-9044-0e82ce3453b6" />


```text
screenshot/01-whois.png
```

### Findings

┌──(kali㉿kali)-[~] <br>
└─$ whois networkwalks.com <br>
   Domain Name: NETWORKWALKS.COM <br>
   Registry Domain ID: 2452319255_DOMAIN_COM-VRSN <br>
   Registrar WHOIS Server: whois.godaddy.com <br>
   Registrar URL: http://www.godaddy.com <br>
   Updated Date: 2025-11-12T10:08:43Z <br>
   Creation Date: 2019-11-06T22:51:46Z <br>
   Registry Expiry Date: 2027-11-06T22:51:46Z <br>
   Registrar: GoDaddy.com, LLC <br>
   Registrar IANA ID: 146 <br>
   Registrar Abuse Contact Email: abuse@godaddy.com  <br>
   Registrar Abuse Contact Phone: 480-624-2505 <br>
   Domain Status: clientDeleteProhibited https://icann.org/epp#clientDelete <br>


---

# 2️⃣ NSLOOKUP Analysis

## Purpose

NSLOOKUP is used to query DNS records and verify domain resolution.

### Command

```bash
nslookup networkwalks.com
```

### Evidence

📸 <img width="348" height="175" alt="nslookup" src="https://github.com/user-attachments/assets/6325680f-d714-4302-840d-01995ae12a25" />


```text
screenshot/02-nslookup.png
```

### Findings

──(root㉿kali)-[/home/kali]<br>
└─# nslookup networkwalks.com   <br>                                            
Server:         10.11.12.13<br>
Address:        10.11.12.13#53<br>
<br>
Non-authoritative answer:<br>
Name:   networkwalks.com<br>
Address: 192.232.216.135<br>


---

# 3️⃣  cURL Header Analysis

## Purpose

cURL was used to inspect HTTP response headers.

### Command

```bash
curl -I https://networkwalks.com
```

### Evidence

📸<img width="1086" height="340" alt="curl" src="https://github.com/user-attachments/assets/7b6056ba-0ff2-4fcd-ba69-d07ab6940bc7" />


```text
screenshot/03-curl.png
```

### Findings


┌──(root㉿kali)-[/home/kali]<br>
└─# curl -I https://networkwalks.com<br>
HTTP/2 200 <br>
permissions-policy: private-state-token-redemption=(self "https://www.google.com" "https://www.gstatic.com" "https://recaptcha.net" "https://challenges.cloudflare.com" "https://hcaptcha.com"), private-state-token-issuance=(self "https://www.google.com" "https://www.gstatic.com" "https://recaptcha.net" "https://challenges.cloudflare.com" "https://hcaptcha.com")<br>
link: <https://networkwalks.com/wp-json/>; rel="https://api.w.org/", <https://networkwalks.com/wp-json/wp/v2/pages/53>; rel="alternate"; title="JSON"; type="application/json", <https://networkwalks.com/>; rel=shortlink<br>
set-cookie: __wpdm_client=edfdc7a600c2ac4852b4c5928c2c9acb; path=/; domain=networkwalks.com; secure; HttpOnly<br>
referrer-policy: no-referrer-when-downgrade<br>
x-endurance-cache-level: 0<br>
x-nginx-cache: WordPress<br>
content-type: text/html; charset=UTF-8<br>
date: Wed, 19 Aug 2026 04:06:13 GMT<br>
server: Apache<br>


---

# 4️⃣ WHATWEB Analysis

## Purpose

WhatWeb identifies technologies used by a website.

### Command

```bash
whatweb https://networkwalks.com
```

### Evidence

📸 <img width="1116" height="261" alt="Whatweb" src="https://github.com/user-attachments/assets/01fd67f7-bc35-4d71-93ef-823952795acf" />



```text
screenshot/04-whatweb.png
```

### Findings

						WhatWeb
                                                                  
┌──(root㉿kali)-[/home/kali]<br>
└─# whatweb networkwalks.com <br>
http://networkwalks.com [301 Moved Permanently] Apache, Cookies[__wpdm_client], Country[UNITED STATES][US], HTTPServer[Apache], HttpOnly[__wpdm_client], IP[192.232.216.135], RedirectLocation[https://networkwalks.com/], UncommonHeaders[permissions-policy,x-redirect-by,upgrade,referrer-policy,x-endurance-cache-level,x-nginx-cache]<br>
https://networkwalks.com [200 OK] Apache, Bootstrap[7.0.4], Cookies[__wpdm_client], Country[UNITED STATES][US], Email[info@networkwalks.com], Frame, Google-Tag-Manager, HTML5, HTTPServer[Apache], HttpOnly[__wpdm_client], IP[192.232.216.135], JQuery[3.7.1], MetaGenerator[WordPress 7.0.4,WordPress Download Manager 3.3.58], Open-Graph-Protocol[website], Script[4684NR-IPIB&amp;pidnVar2=50511&amp;prtVar2=7&amp;scvVar2=12,application/json,application/ld+json,module,speculationrules,text/javascript], Title[Networkwalks Academy], UncommonHeaders[permissions-policy,link,upgrade,referrer-policy,x-endurance-cache-level,x-nginx-cache], WordPress[7.0.4]<br>
https://networkwalks.com/ [200 OK] Apache, Bootstrap[7.0.4], Country[UNITED STATES][US], Email[info@networkwalks.com], Frame, Google-Tag-Manager, HTML5, HTTPServer[Apache], IP[192.232.216.135], JQuery[3.7.1], MetaGenerator[WordPress 7.0.4,WordPress Download Manager 3.3.58], Open-Graph-Protocol[website], Script[4684NR-IPIB&amp;pidnVar2=50511&amp;prtVar2=7&amp;scvVar2=12,application/json,application/ld+json,module,speculationrules,text/javascript], Title[Networkwalks Academy], UncommonHeaders[permissions-policy,link,upgrade,referrer-policy,x-endurance-cache-level,x-nginx-cache], WordPress[7.0.4]     <br>                                        

---

# 5️⃣ WAFW00F Analysis

## Purpose

Wafw00f detects Web Application Firewall protections.

### Command

```bash
wafw00f https://networkwalks.com
```

### Evidence

📸 <img width="757" height="399" alt="WAF" src="https://github.com/user-attachments/assets/be525b6e-46b3-4f8a-81df-471a18cf711d" />


```text
screenshot/05-wafw00f.png
```

### Findings

┌──(root㉿kali)-[/home/kali]<br>
└─# wafw00f networkwalks.com       <br>                                       

                   ______
                  /      \
                 (  Woof! )
                  \  ____/                      )
                  ,,                           ) (_
             .-. -    _______                 ( |__|
            ()``; |==|_______)                .)|__|
            / ('        /|\                  (  |__|
        (  /  )        / | \                  . |__|
         \(_)_))      /  |  \                   |__|

                    ~ WAFW00F : v2.3.2 ~
    The Web Application Firewall Fingerprinting Toolkit                                                                     
                                                                                                                            
[*] Checking https://networkwalks.com<br>
[+] The site https://networkwalks.com is behind ModSecurity (SpiderLabs) WAF.<br>
[~] Number of requests: 2<br>


---

# 📊 Reconnaissance Summary

| Tool | Information Gathered |
|--------|---------------------|
| WHOIS | Domain registration information |
| NSLOOKUP | DNS resolution details |
| cURL | HTTP response headers |
| WhatWeb | Website technologies |
| Wafw00f | WAF detection results |


---

# 🧠 Key Learning Outcomes

Through this exercise, I gained hands-on experience with:

- Information Gathering
- Footprinting Methodologies
- DNS Enumeration
- Domain Intelligence Collection
- Technology Fingerprinting
- Web Security Analysis
- HTTP Header Inspection
- Security Documentation
- Professional Reporting

---

# 📸 Evidence Gallery

### WHOIS

📸 screenshots/01-whois.png

### NSLOOKUP

📸 screenshots/02-nslookup.png

###  CURL

📸 screenshots/03-curl.png

### WHATWEB

📸 screenshots/04-whatweb.png

### WAFW00F

📸 screenshots/05-wafw00f.png


---

# ⚖️ Ethics Statement

This project was conducted strictly within the authorized scope provided by the NetworkWalks Cybersecurity Internship Program.

No exploitation, unauthorized access, denial-of-service attacks, password attacks, or malicious activities were performed.

The objective of this exercise was educational learning and professional skill development.

---

# 👨‍💻 Author

**Balwant Singh**

Cybersecurity Student

NetworkWalks Cybersecurity Internship — Batch B082

GitHub: [ADD GITHUB PROFILE]

LinkedIn: [ADD LINKEDIN PROFILE]

---

<div align="center">

### 🔐 Ethical Reconnaissance • Responsible Learning • Continuous Improvement

</div>
