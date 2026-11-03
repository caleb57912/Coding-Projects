# OSINT Web Scraper

Collects open-source information about a target from public web pages.

## Problem

A lot of reconnaissance is reading public pages and pulling out the useful parts — links, email addresses, technologies, references. This automates that gathering and the parsing.

## Libraries

`requests` (fetch pages) · `beautifulsoup4` (parse HTML) · `re` (extract emails, patterns) · `scrapy` (rebuild as a real crawler in M4)

## Build plan

- [ ] **M1** Fetch one page with `requests`; check status and encoding
- [ ] **M2** Parse it with BeautifulSoup; extract links and emails with `re`
- [ ] **M3** Crawl within scope: stay on-domain, limit depth, respect `robots.txt`
- [ ] **M4** Rebuild the crawler as a Scrapy spider
- [ ] **M5** Output structured results (CSV / JSON)

## Done when

Given a starting URL and a scope, it returns a structured set of pages and the data pulled from them, politely.

## Rules

Scrape only sites you're authorized to, honor `robots.txt` and rate limits, and don't collect personal data you have no reason to hold.
