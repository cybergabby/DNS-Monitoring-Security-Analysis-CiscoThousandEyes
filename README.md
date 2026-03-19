# DNS-Monitoring-Security-Analysis-CiscoThousandEyes
Global DNS Monitoring &amp; Security Analysis using Cisco ThousandEyes

# Project Overview

This project demonstrates how to monitor and analyze DNS performance, availability, and security using Cisco ThousandEyes.
The objective was to evaluate how a public domain (google.com) resolves across different global locations, identify potential DNS issues, and assess security mechanisms such as DNSSEC.

# Objectives

Monitor DNS availability from multiple global agents
Measure DNS query performance (latency)
Analyze DNSSEC validation status
Identify potential security gaps in DNS resolution
Understand real-world DNS behavior from a security perspective

# Lab Setup

Tool: Cisco ThousandEyes

Test Type: DNS Test (A Record)

Target: google.com

Protocol: UDP

Agents: Global (multiple regions)

<img width="1366" height="682" alt="DNS servertest2" src="https://github.com/user-attachments/assets/84803f30-2265-4c00-9d8a-8d27b280feb9" />

<img width="1366" height="659" alt="DNS Server Test" src="https://github.com/user-attachments/assets/6181e56f-c3b2-4b4f-93d3-515a8463fe68" />

# Key Metrics Analyzed
1. Availability

Result: 100%
Insight: DNS resolution was successful across all test locations

2. Query Time
Result: ~44 ms
Insight: Fast DNS response time indicating optimal performance

3. DNSSEC Validation
Result: 0% Validity
Insight: No DNSSEC public keys detected

Indicates DNSSEC is not enforced for this query

<img width="1366" height="659" alt="DNS server3" src="https://github.com/user-attachments/assets/097970a1-8fcc-4186-b999-89119c868bfa" />


# Global Visibility

Using distributed agents, the test provided insight into how DNS behaves across different geographic regions, helping identify location-based failures or inconsistencies.

# Security Analysis

 Findings:
DNS resolution is stable and globally available
Lack of DNSSEC validation could expose DNS queries to:

Spoofing attacks
Cache poisoning
Man-in-the-middle (MITM) risks


<img width="1365" height="661" alt="dns sec" src="https://github.com/user-attachments/assets/e0ee99d9-2e6a-4eb1-88f0-f6ace7d595e5" />

# Detection & Monitoring Use Cases

This setup can be used to detect:

DNS hijacking attempts
Unexpected IP resolution changes
Regional DNS outages
Suspicious latency spikes

# Key Skills Demonstrated

Network Monitoring
DNS Analysis
Security Visibility
Performance Analysis
Threat Detection Thinking

# Conclusion

This project highlights how DNS monitoring tools like Cisco ThousandEyes can be used not only for performance tracking but also for identifying potential security risks and improving visibility across global network infrastructure.

