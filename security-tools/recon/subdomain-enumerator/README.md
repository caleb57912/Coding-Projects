# Subdomain Enumerator

Finds live subdomains of a domain from a wordlist.

## Problem

Mapping an organization's attack surface starts with finding what hostnames exist. This does it the simplest way: guess `word.domain.com`, resolve it, keep the ones that answer.

## Libraries

`socket` (DNS resolution) · `requests` (check which resolve to a live site) · `re` (validate hostnames, strip duplicates) · concurrency

## Build plan

- [ ] **M1** Resolve one hostname to an IP
- [ ] **M2** Read a wordlist and build candidate subdomains
- [ ] **M3** Add concurrency; handle names that don't resolve cleanly
- [ ] **M4** For resolved names, check HTTP/HTTPS status with `requests`
- [ ] **M5** Handle wildcard DNS, dedupe, output results

## Done when

Given a domain and a wordlist, it returns the subdomains that resolve and which of those serve a live site.

## Rules

Only enumerate domains you own or are authorized to test.
