<div align="center">

# 💻 Coding Projects

**The code I write to get better at programming and to solve real security and IT problems.**

<img src="https://img.shields.io/badge/Status-Getting_started-F2A900?style=for-the-badge">
<img src="https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white">
<img src="https://img.shields.io/badge/Focus-Security_Tooling-C8202F?style=for-the-badge">

</div>

---

> ### 📖 Start here: [**Security Tools →**](security-tools/)
> The first theme: Python tools for recon, log analysis, automation, threat intel and forensics.

## 🎯 Mission

Become as fluent in Python as I am in English, and use it to build tools I'd actually run on the job.

I work in IT operations at an MSP and run a SOC, RMM and GRC program on my home network. Every project here starts from a real task in that work: something I did by hand, a gap in a tool, or a question I wanted answered from data.

## 🧩 How this repo is organized

Projects are grouped into themes. Each theme has its own folder, its own index and its own README.

| Theme | Focus | Status |
| --- | --- | --- |
| [**Security Tools**](security-tools/) | Recon, log analysis, automation, threat intel and forensics tooling | 🚧 Active |
| Scripting & Automation | General IT and sysadmin scripts outside security | 🔜 Planned |
| Fundamentals | Exercises and small programs that build core Python skills | 🔜 Planned |

## 🗂️ Project index

| Project | Theme | What it does | Status |
| --- | --- | --- | --- |
| [port-scanner](security-tools/recon/port-scanner) | Security Tools · recon | TCP port scanner on raw sockets | 🚧 Building |
| [subdomain-enumerator](security-tools/recon/subdomain-enumerator) | Security Tools · recon | Finds live subdomains from a wordlist | 🔜 Planned |
| [hash-cracker](security-tools/forensics/hash-cracker) | Security Tools · forensics | Dictionary / brute-force hash recovery | 🔜 Planned |
| [osint-web-scraper](security-tools/recon/osint-web-scraper) | Security Tools · recon | Collects OSINT from public pages | 🔜 Planned |
| [nmap-automapper](security-tools/recon/nmap-automapper) | Security Tools · recon | Drives Nmap across targets, reports results | 🔜 Planned |

See the [Security Tools roadmap](security-tools/ROADMAP.md) for build order and the library map.

## 📐 Project standards

Every project folder follows the same shape, from [`_templates/project-README.md`](_templates/project-README.md):

| Section | Purpose |
| --- | --- |
| **Problem** | The real task or question that started it |
| **Usage** | How to install and run it, with an example |
| **How it works** | The design, and the Python concepts it uses |
| **What I learned** | Mistakes, fixes and what I'd change |

Each project pins its dependencies in its own `requirements.txt` and runs in its own virtual environment.

## 🔗 Related work

| Repo | Focus |
| --- | --- |
| [SOC-Homelab](https://github.com/caleb57912/SOC-Homelab) | Detect and respond: SIEM, endpoint and network telemetry, threat intel |
| [RMM-Homelab](https://github.com/caleb57912/RMM-Homelab) | Manage and automate: inventory, patching, scripting, remote access |
| [GRC-Homelab](https://github.com/caleb57912/GRC-Homelab) | Govern: policies, CIS Controls v8 assessment, risk register, compliance reporting |
| [AWS-Migration-Design](https://github.com/caleb57912/AWS-Migration-Design) | Cloud architecture: healthcare workload migration design and cost estimate |

Tools built here get used in those labs, and the labs supply the data and problems these tools are built for.

## 📁 Repository map

| Folder | What's inside |
| --- | --- |
| [`security-tools/`](security-tools) | **Security tooling, grouped by domain** |
| [`_templates/`](_templates) | README template for new projects |

## 🔒 Privacy & sanitization

Tools here are tested against my own network and lab. Sample data, logs and screenshots have public IPs, domain names, credentials and API keys removed before they're published. Redacted values appear as `<REDACTED>`. Keys and secrets are read from environment variables, never hardcoded.

---

<div align="center">

**Caleb Santora** · Security+ · CySA+ · SecurityX · Associate of ISC2

[GitHub Profile](https://github.com/caleb57912)

</div>
