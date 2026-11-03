# 🛠️ Security Tools

Python tools for security work. Each one starts from a task I'd otherwise do by hand in the SOC, RMM or GRC labs, or on the job.

> 📖 [**Roadmap →**](ROADMAP.md) — the five tools in this theme, in build order, with status.

## Domains

| Folder | Focus | Examples of what belongs here |
| --- | --- | --- |
| [`recon/`](recon) | Discovery and enumeration | Port scanners, subdomain enumeration, Nmap automation, OSINT gathering |
| [`log-analysis/`](log-analysis) | Parsing and finding signal in logs | Auth log parsers, Sysmon event summaries, Pi-hole query analysis |
| [`automation/`](automation) | Removing repeated manual work | API clients for Splunk, TheHive or Wazuh, report generators |
| [`threat-intel/`](threat-intel) | Working with IoCs and reputation data | IoC extractors, VirusTotal and AbuseIPDB lookups, MISP queries |
| [`forensics/`](forensics) | Triage and evidence handling | File hashing, hash cracking, metadata extraction, timeline building |

## Index

| Project | Domain | What it does | Status |
| --- | --- | --- | --- |
| [port-scanner](recon/port-scanner) | recon | TCP port scanner on raw sockets | 🚧 Building |
| [subdomain-enumerator](recon/subdomain-enumerator) | recon | Finds live subdomains from a wordlist | 🔜 Planned |
| [nmap-automapper](recon/nmap-automapper) | recon | Drives Nmap across a target list, reports results | 🔜 Planned |
| [osint-web-scraper](recon/osint-web-scraper) | recon | Collects OSINT from public pages | 🔜 Planned |
| [hash-cracker](forensics/hash-cracker) | forensics | Dictionary / brute-force hash recovery | 🔜 Planned |

## Rules for these tools

- Run only against systems I own or am authorized to test.
- API keys come from environment variables, never from the code.
- Sample data in the repo is sanitized; redacted values appear as `<REDACTED>`.
