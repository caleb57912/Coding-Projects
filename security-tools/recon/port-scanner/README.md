# Port Scanner

A TCP port scanner built on raw sockets.

## Problem

Nmap already does this. The point is to understand what a scanner actually does under the hood — open a socket, attempt a connection, read the result — before automating Nmap in a later project.

## Libraries

`socket` (connections) · `argparse` (CLI) · `re` (input validation) · `multiprocessing` or `threading` (concurrency)

## Build plan

- [ ] **M1** Connect to one port on one host, print open or closed
- [ ] **M2** Scan a port range; take host + ports from the command line; validate the input
- [ ] **M3** Add concurrency and a per-connection timeout
- [ ] **M4** Grab the service banner from open ports
- [ ] **M5** Format output (table / JSON) and write up the README

## Done when

You can run it against a host in your lab, get a list of open ports with services in a few seconds, and explain every design choice.

## Rules

Scan only hosts you own or are authorized to test — your own lab. Nothing on this list is to be pointed at systems you don't control.
