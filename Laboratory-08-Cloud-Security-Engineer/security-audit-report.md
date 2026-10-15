# Security Audit Report

## Core Security Concepts 

### 1. The Principle of Least Privilege (PoLP)
The Principle of Least Privilege dictates that users, processes, and systems should only be granted the minimum level of access and permissions required to perform their specific tasks. This is vital for cloud user accounts because it restricts the blast radius if an account is compromised, preventing attackers from gaining broader administrative control over the entire infrastructure.

### 2. Attack Surface
An attack surface refers to the sum total of all exposed entry points, open network ports, active services, and potential vulnerabilities on a virtual machine that an unauthorized user could exploit. Minimizing this surface by closing unused ports directly reduces the available entry vectors for malicious actors.

### 3. Default Deny Policy
A default deny policy blocks all incoming network traffic automatically by default and only permits specifically authorized connections. It is far safer than trying to block specific hackers individually because it provides immediate protection against unknown, emerging, or future threats without requiring a pre-existing list of malicious IP addresses.
