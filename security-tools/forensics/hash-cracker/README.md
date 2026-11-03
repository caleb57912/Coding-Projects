# Hash Cracker

Recovers the input behind a password hash by dictionary and brute-force search — a tool for understanding why weak password hashing fails.

## Problem

Knowing that `hashlib` turns a password into a hash is one thing; seeing how fast a weak hash falls to a wordlist is what makes password and hashing policy real. This also exercises CPU-bound parallelism with `multiprocessing`.

## Libraries

`hashlib` (hashing) · `multiprocessing` (parallel search) · `argparse` (CLI) · file I/O (wordlist)

## Build plan

- [ ] **M1** Hash a candidate string and compare it to a target hash
- [ ] **M2** Dictionary attack: try every word in a wordlist
- [ ] **M3** Accept the hash type (md5 / sha1 / sha256); handle salts
- [ ] **M4** Parallelize the search with `multiprocessing`
- [ ] **M5** Report progress and rate; print the result cleanly

## Done when

Given a hash, its type, and a wordlist, it finds the matching input if the wordlist contains it, using all your cores.

## Rules

Only crack hashes from your own systems or test data — test your own password strength, or lab accounts you control. Not for credentials you don't own.
