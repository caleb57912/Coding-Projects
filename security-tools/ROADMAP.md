# Security Tools — Roadmap

Five Python tools, in the order I'm building them. Each links to its own build plan.

| # | Tool | Domain | Core libraries | Status |
| --- | --- | --- | --- | --- |
| 1 | [Port Scanner](recon/port-scanner) | recon | socket, multiprocessing, re | 🚧 Building |
| 2 | [Subdomain Enumerator](recon/subdomain-enumerator) | recon | socket, requests, re | 🔜 Planned |
| 3 | [Hash Cracker](forensics/hash-cracker) | forensics | hashlib, multiprocessing | 🔜 Planned |
| 4 | [OSINT Web Scraper](recon/osint-web-scraper) | recon | requests, beautifulsoup4, scrapy, re | 🔜 Planned |
| 5 | [Nmap Automapper](recon/nmap-automapper) | recon | subprocess, re | 🔜 Planned |

## Library map

What each library is for, and which tools use it.

| Library | Used for | Tools |
| --- | --- | --- |
| `socket` | Raw TCP connections, DNS resolution | Port Scanner, Subdomain Enumerator |
| `subprocess` | Running external tools (Nmap) | Nmap Automapper |
| `requests` | HTTP requests | Subdomain Enumerator, OSINT Web Scraper |
| `beautifulsoup4` | Parsing HTML | OSINT Web Scraper |
| `scrapy` | Full crawling framework | OSINT Web Scraper (advanced stage) |
| `multiprocessing` | Parallelism for CPU- and connection-bound work | Hash Cracker, Port Scanner |
| `re` | Input validation, output parsing, pattern extraction | All five |
| `hashlib` | Hashing | Hash Cracker |
| `paramiko` | SSH sessions | Not yet assigned — candidate for a future SSH audit / config-backup tool |

> `paramiko` isn't needed by any of the first five. It's on the learning list, so it gets its own project later (e.g. an SSH login auditor or a switch-config backup tool for the RMM lab).
