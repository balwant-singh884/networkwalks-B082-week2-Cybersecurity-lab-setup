<div align="center">

# 🔐 NETWORKWALKS CYBERSECURITY INTERNSHIP

## Week 02 – Footprinting & Network Scanning

### W2-PM1 • W2-PM5 • W2-PM-FINAL

![Kali Linux](https://img.shields.io/badge/Kali-Linux-blue?style=for-the-badge&logo=kalilinux)
![VMware](https://img.shields.io/badge/VMware-Workstation-orange?style=for-the-badge&logo=vmware)
![NetworkWalks](https://img.shields.io/badge/Batch-B082-success?style=for-the-badge)
![Reconnaissance](https://img.shields.io/badge/Footprinting-Completed-brightgreen?style=for-the-badge)
![Zenmap](https://img.shields.io/badge/Zenmap-Completed-blue?style=for-the-badge)
![Report](https://img.shields.io/badge/Final_Report-Completed-purple?style=for-the-badge)

<br>

### Ethical Reconnaissance • Network Discovery • Security Documentation

</div>

---

# 📌 Project Overview

This repository contains the work completed during **Week 02** of the **NetworkWalks Cybersecurity Internship (Batch B082)**.

The assessment focused on two primary cybersecurity activities:

- Passive & Active Footprinting
- Network Discovery & Enumeration using Zenmap

The objective was to collect publicly available information about an authorized target, analyze DNS and web technologies, identify reachable hosts within an authorized network, and document findings professionally.

---

# 📜 Authorization & Scope

This assessment was conducted under the authorization provided by **NetworkWalks**.

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

✅ DNSRecon

✅ Nmap / Zenmap Host Discovery

✅ Network Topology Mapping




### Prohibited Activities

❌ Exploitation

❌ Denial of Service

❌ Brute Force Attacks

❌ Unauthorized Access Attempts

❌ Privilege Escalation

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
| DNSRecon | DNS enumeration |
| Zenmap | Host Discovery |
| Nmap | Network Enumeration |



---

# 📂 Repository Structure

```text
networkwalks-B082-week2-footprinting-reconnaissance
│
├── README.md
│
├── authorization
│   
│   
│
├── screenshots
|   ├── 01-whois.png
|   ├── 02-nslookup.png
|   ├── 03-curl.png
|   ├── 04-whatweb.png
|   ├── 05-wafw00f.png
|   └── 06-DNSRecon.png
└── zenmap
│       ├── 01-ipconfig.png
│       ├── 02-host-discovery.png
│       ├── 03-live-hosts.png
│       ├── 04-ip-addresses.png
│       ├── 05-mac-addresses.png
│       ├── 06-topology.png
│       └── network-topology.pdf
│
├── results
    │
    ├── footprinting
    └── zenmap


---
# 🔎 Module 1 — Footprinting & Reconnaissance (W2-PM1)

## Objective

Perform authorized reconnaissance against the target domain using multiple Kali Linux information-gathering tools.


# 🔎 Reconnaissance Workflow

```text
                          Target
                             │
                             ▼
                  Reconnaissance Phase
                             │
                             ▼
      ┌──────────────────────────────────────┐
      │              Footprinting            │
      └──────────────────────────────────────┘
                             │
                             ▼
        WHOIS → NSLOOKUP → DNSRECON
                             │
                             ▼
         WHATWEB → WAFW00F → CURL
                             │
                             ▼
              Information Collection
                             │
                             ▼
      ┌──────────────────────────────────────┐
      │        Network Scanning Phase        │
      └──────────────────────────────────────┘
                             │
                             ▼
                   Network Configuration
                             │
                             ▼
                      Host Discovery
                             │
                             ▼
                   Live Host Analysis
                             │
                             ▼
                 Port / Service Discovery
                             │
                             ▼
                    Topology Mapping
                             │
                             ▼
      ┌──────────────────────────────────────┐
      │          Reporting Phase             │
      └──────────────────────────────────────┘
                             │
                             ▼
                    Evidence Collection
                             │
                             ▼
                     Results Analysis
                             │
                             ▼
                    Findings Summary
                             │
                             ▼
                  Final Assessment Report
```

---

# 🔍 Module 1 — Footprinting & Reconnaissance (W2-PM1)

## 1️⃣ WHOIS Analysis

### Purpose

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
# 6️⃣ DNSRECON Analysis

## Purpose

DNSRecon performs DNS enumeration and information gathering.

### Command

```bash
dnsrecon -d networkwalks.com
```

### Evidence

📸 <img width="1900" height="527" alt="Screenshot 2026-08-20 000304" src="https://github.com/user-attachments/assets/a117db22-b52a-4790-b5b8-5286401d7018" />




```text
screenshot/06-dnsrecon.png
```

### Findings

                                                                                              
┌──(kali㉿kali)-[~]<br>
└─$ dnsrecon -d networkwalks.com<br>
2026-08-19T14:09:15.981786-0400 INFO Starting enumeration for domain: networkwalks.com<br>
2026-08-19T14:09:15.982227-0400 INFO std: Performing General Enumeration against: networkwalks.com...<br>
2026-08-19T14:09:19.297523-0400 ERROR No answer for DNSSEC query for networkwalks.com<br>
2026-08-19T14:09:20.829643-0400 INFO     SOA ns6135.hostgator.com 50.87.144.87<br>
2026-08-19T14:09:31.786771-0400 INFO     A networkwalks.com 192.232.216.135<br>
2026-08-19T14:09:38.032341-0400 INFO Enumerating SRV Records<br>
2026-08-19T14:09:48.019864-0400 ERROR No SRV Records Found for networkwalks.com<br>
2026-08-19T14:09:48.020270-0400 INFO Completed enumeration for domain: networkwalks.com<br>


---

# 📊 Reconnaissance Summary

| Tool | Information Gathered |
|--------|---------------------|
| WHOIS | Domain registration information |
| NSLOOKUP | DNS resolution details |
| cURL | HTTP response headers |
| WhatWeb | Website technologies |
| Wafw00f | WAF detection results |
| DNSRecon | DNS records and enumeration |


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


# 🌐 Module 2 — Network Scanning with Zenmap (W2-PM5)

## Objective

Identify active hosts, enumerate network information, and visualize network topology using Zenmap.

---

## 1️⃣ Network Configuration & Scope

### Objective

Identify the local IP address and LAN subnet before performing network discovery. This establishes the scanning range for the authorized assessment.

### Command

```cmd
ipconfig
```

### Evidence

<img src="evidence/zenmap/01-ipconfig.png" width="900">

---

## 2️⃣ Live Host Discovery

### Objective

Identify active hosts within the authorized LAN subnet using Zenmap's Ping Scan.

### Scan Configuration

- **Target:** Local LAN subnet identified in Task 1
- **Profile:** Ping Scan
- **Nmap Scan:** Host Discovery

### Command

```bash
nmap -sn 10.0.0.0/24
```

### Evidence

<img src="evidence/zenmap/02-host-discovery.png" width="900">

---

## 3️⃣ Live Host Count

### Objective

Determine the total number of active hosts identified during the Zenmap host-discovery scan.

### Result

The scan identified **4 live hosts**, including the assessment system.

### Evidence

<img src="evidence/zenmap/03-live-hosts.png" width="900">

---

## 4️⃣ Live Host IP Addresses

### Objective

Record the IPv4 addresses of the hosts identified as active during the Zenmap discovery scan.

### Results

The following hosts were identified as live:

| Host | IP Address |
|------|------------|
| Host 1 | `10.0.0.1` |
| Host 2 | `10.0.0.4` |
| Host 3 | `10.0.0.19` |
| Host 4 | `10.0.0.5` |

### Evidence

<img src="evidence/zenmap/04-ip-addresses.png" width="900">

---

## 5️⃣ Live Host MAC Addresses

### Objective

Record the MAC addresses associated with the live hosts identified during the Zenmap discovery scan.

### Results

| Host | MAC Address |
|------|-------------|
| Host 1 | `00:50:56:E3:B3:2C` |
| Host 2 | `00:0C:29:C0:94:8F` |
| Host 3 | `00:50:56:E9:64:82` |
| Host 4 | `00:0C:29:40:C0:93` |

The fourth MAC address represents the local assessment system and was obtained using the system's network configuration.

### Evidence

<img src="evidence/zenmap/05-mac-addresses.png" width="900">

---

## 6️⃣ Network Topology Mapping

### Objective

Visualize the discovered hosts and network relationships using Zenmap's **Topology** view and preserve the result as supporting assessment evidence.

### Procedure

1. Open the **Topology** tab in Zenmap.
2. Enable the topology legend.
3. Review the displayed network relationships.
4. Save the topology graphic.
5. Select **PDF** as the output format.
6. Store the exported topology with the assessment evidence.

### Evidence

<img src="evidence/zenmap/06-topology.png" width="900">

### Output

**Topology File:**

```text
evidence/zenmap/network-topology.pdf
```

---

# 📊 W2-PM5 Results Summary

| Assessment Item | Result |
|-----------------|---------|
| Live Hosts Identified | **4** |
| Network Discovery | Completed |
| IP Addresses Recorded | **4** |
| MAC Addresses Recorded | **4** |
| Network Topology | Generated and Exported to PDF |
| Scanning Tool | Zenmap / Nmap |
| Assessment Scope | Authorized Local LAN |

---

### Key Takeaway

The Zenmap assessment successfully identified the active hosts within the authorized LAN and documented their IP and MAC addresses. The resulting topology diagram provides a visual representation of the discovered network and has been preserved as supporting evidence.

### Evidence

Zenmap scan output, host information, screenshots, and the exported topology PDF are maintained under:

```text
evidence/zenmap/
```

---



# 📋 Module 3 — Final Assessment Report (W2-PM-FINAL)

## Executive Summary

This assessment was conducted as part of the NetworkWalks Cybersecurity Internship (Batch B082) and focused on authorized reconnaissance and network discovery activities.

The objective was to gather publicly available information about the target environment, analyze DNS and web technologies, identify reachable hosts within the authorized network, and document findings using industry-standard reconnaissance and network-scanning methodologies.

The assessment combined both passive and active information-gathering techniques through footprinting tools and Zenmap-based network discovery.

---

## Assessment Scope

### Authorized Target

```text
networkwalks.com
```

### Assessment Activities

- Domain Intelligence Gathering
- DNS Enumeration
- Technology Fingerprinting
- WAF Detection
- HTTP Header Analysis
- Host Discovery
- Network Enumeration
- Network Topology Mapping
- Evidence Collection
- Security Documentation

### Assessment Constraints

The following activities were outside the scope of this assessment and were not performed:

- Vulnerability Scanning
- Exploitation
- Brute Force Attacks
- Privilege Escalation
- Denial of Service Testing
- Unauthorized Access Attempts

---

## Assessment Methodology

The assessment followed a structured three-phase approach:

### Phase 1 — Reconnaissance

Information gathering was conducted using:

- WHOIS
- NSLOOKUP
- DNSRecon
- WhatWeb
- Wafw00f
- cURL

These tools were used to collect publicly available information regarding domain registration, DNS records, web technologies, security controls, and HTTP response characteristics.

---

### Phase 2 — Network Discovery

Network scanning activities were conducted using Zenmap and Nmap.

The assessment included:

- Network configuration verification
- Host discovery
- Live host identification
- IP address enumeration
- MAC address collection
- Network topology generation

---

### Phase 3 — Reporting & Documentation

Assessment evidence was collected, organized, and documented throughout the engagement.

The final report was prepared to provide:

- Assessment objectives
- Methodology
- Findings
- Supporting evidence
- Summary observations

---

## Reconnaissance Findings Summary

The footprinting phase successfully collected information related to:

| Area | Description |
|--------|-------------|
| WHOIS | Domain registration information |
| DNS Resolution | Domain-to-IP resolution |
| DNS Enumeration | DNS record discovery |
| Technology Fingerprinting | Web technologies in use |
| WAF Detection | Presence of web application protection |
| HTTP Analysis | Response headers and server information |

The collected information provided insight into the target's publicly accessible infrastructure and technology stack.

---

## Network Discovery Findings Summary

The Zenmap assessment successfully identified active hosts within the authorized assessment network.

### Results

| Assessment Item | Result |
|-----------------|---------|
| Live Hosts Identified | 4 |
| IP Addresses Recorded | 4 |
| MAC Addresses Recorded | 4 |
| Network Topology Generated | Yes |
| Topology Exported | PDF |

### Network Information Collected

| Host | IP Address |
|--------|------------|
| Host 1 | 10.0.0.1 |
| Host 2 | 10.0.0.4 |
| Host 3 | 10.0.0.19 |
| Host 4 | 10.0.0.5 |

The resulting topology diagram provided a visual representation of the discovered network environment.

---

## Cross-Phase Analysis

The assessment combined both reconnaissance and network-discovery activities to provide multiple perspectives of the authorized environment.

### External Perspective

The footprinting phase provided visibility into:

- Domain ownership information
- DNS infrastructure
- Web technologies
- Security controls
- HTTP response behavior

### Internal Perspective

The network-scanning phase provided visibility into:

- Reachable hosts
- Network addressing
- MAC address information
- Network topology

Together, these activities established a baseline understanding of the assessed environment.

---

## Key Learning Outcomes

Through this assessment, the following practical skills were developed:

- Domain Footprinting
- DNS Enumeration
- Technology Fingerprinting
- WAF Identification
- HTTP Header Analysis
- Host Discovery
- Network Enumeration
- Topology Mapping
- Evidence Collection
- Technical Documentation
- Professional Reporting

---

## Evidence Management

All evidence generated during the assessment has been organized and retained within the repository.

### Evidence Directory

```text
evidence/
├── footprinting/
├── zenmap/
└── network-topology.pdf
```

### Results Directory

```text
results/
├── footprinting/
└── zenmap/
```

The evidence includes screenshots, command outputs, topology exports, and supporting documentation.

---

## Assessment Conclusion

The Week 02 assessment successfully achieved its objectives by combining authorized footprinting and network discovery activities.

Reconnaissance techniques provided valuable information regarding domain registration, DNS infrastructure, web technologies, security controls, and HTTP response characteristics. Network scanning activities successfully identified active hosts, recorded network information, and generated a visual topology of the authorized environment.

The assessment demonstrates the practical application of information-gathering and network-discovery methodologies while maintaining compliance with the authorized scope defined by NetworkWalks.

The collected evidence and documented findings provide a structured baseline that can support future security assessments, network analysis activities, and cybersecurity learning objectives.

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

LinkedIn: inkedin.com/in/balwant-singh-a5a4a232b/

---

<div align="center">

### 🔐 Ethical Reconnaissance • Responsible Learning • Continuous Improvement

</div>
