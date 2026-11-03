# Nmap Automapper

Wraps Nmap to scan a list of targets and turn the output into a clean report.

## Problem

Running Nmap by hand across many hosts and reading raw output is slow. This drives Nmap programmatically and parses the results into something searchable — and ties back to the port-scanner project by comparing findings.

## Libraries

`subprocess` (run Nmap) · `re` (build and validate arguments, parse output) · file I/O for storing results

## Build plan

- [ ] **M1** Run a fixed Nmap command with `subprocess`, capture its output
- [ ] **M2** Build the command from CLI arguments; validate targets and flags
- [ ] **M3** Parse the output into structured data (prefer `-oX` XML over scraping text)
- [ ] **M4** Loop over a target list; store each result
- [ ] **M5** Produce a summary report; cross-check against port-scanner output

## Done when

You point it at a target file, it runs Nmap per host, and you get a single structured report.

## Rules

Nmap only against hosts you own or are authorized to test. Requires Nmap installed on the host.
