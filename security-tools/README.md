# 🛠️ Security Tools

Python tools for security work. Each one starts from a task I'd otherwise do by hand in the SOC, RMM or GRC labs, or on the job.

## Domains

| Folder | Focus | Examples of what belongs here |
| --- | --- | --- |
| [`recon/`](recon) | Discovery and enumeration | Port scanners, service banner grabbers, subnet sweeps, DNS lookups |
| [`log-analysis/`](log-analysis) | Parsing and finding signal in logs | Auth log parsers, Sysmon event summaries, Pi-hole query analysis |
| [`automation/`](automation) | Removing repeated manual work | API clients for Splunk, TheHive or Wazuh, report generators |
| [`threat-intel/`](threat-intel) | Working with IoCs and reputation data | IoC extractors, VirusTotal and AbuseIPDB lookups, MISP queries |
| [`forensics/`](forensics) | Triage and evidence handling | File hashing, metadata extraction, timeline building |

## Index

| Project | Domain | What it does | Status |
| --- | --- | --- | --- |
| *None yet* | | | |

## Rules for these tools

- Run only against systems I own or am authorized to test.
- API keys come from environment variables, never from the code.
- Sample data in the repo is sanitized; redacted values appear as `<REDACTED>`.
